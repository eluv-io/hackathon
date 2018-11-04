

# Set up the application

## Create a library

client = ElvClient(...)

libraryID = client.CreateContentLibrary("some name", "some description", signer)

- need to get contract address (which is different from libraryID)


# Create a new contract for a new piece of contnent

1. Create your smart contract

client.ethClient.DeployContract({abi: YOURABI, bytecode: YOURBINARY, ARGS, signer)

Where ARGS is a JSON list: [ ARG1, ARG2, ...]

Remember the custom contract ADDRESS


2. Create the base content contract

client.ethClient.CallContractMethod(library contract,  abi, "createContent", ARGS, signer)

- TODO ARGS
- get the contract address from the EVENT


3. Create fabric object

- CreateContentObject( libraryId, OPTIONS)


4. Set the custom contract

await cont.setCustomContractAddress(CUSTOM_CONTRACT_ADDRESS);


# Operate on the content

- Can call methods on the custom cuntract you made

client.ethClient.CallContractMethod(library contract,  abi, yourmethod, ARGS, signer)


- Store deta in the content object

First EditContentObject()

    output += "EDITING " + objectId + "...\n";
    let editResponse = await client.EditContentObject({
      libraryId: libraryId,
      contentId: objectId,
      options: {
        meta: {
          "meta": "changed",
          "sub": {
            "tree": "value"
          }
        }
      }
    });


Then MergeMetaData

    await client.MergeMetadata({
      libraryId,
      writeToken: editResponse.write_token,
      metadata: { newField: "newValue"}
    });


When done Finalize

    await (
      client.FinalizeContentObject({
        libraryId,
        writeToken: editResponse.write_token
      })
    );

