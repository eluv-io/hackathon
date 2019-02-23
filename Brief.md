Eluvio if building a novel, Internet-scale plafrom for large form-content, built for media from the ground up.

Media content is controlled by an Ethereum-compatible blockchain through smart contracts.

Push your content and your code that operates on the content, then designate the smart contract governing 
access to your application and you are online and ready for 10 users or 10 million users.  No storage, databases,
transcoding pipelines or servers.

Visit https://github.com/eluv-io/hackathon for info on the API challenge, docs and sample code.

## API info and challenge

Developing an application for the Eluvio content fabric consists of writing
(a) The content 'bitcode' - this is code that operates on the content itself and is published into the fabric and will be
executed by any fabric node as necessary (for example code that creates a 10 second trailer from a video clip, puts glasses and moustaches on characters or counts the number of key frames)
(b) The smart contract (Ethereum Solidity) which implements the logic that allows uses to access the content, pay or get paid, etc
(c) The front end application which uses the content fabric API as a backend (no other backend necessry unless specifically desired)

The Eluvio API challenge consists of creating an application that utilizes all these three categories of code and has at least two type of users (for example content owners, consumers, advertizers, publishers, service providers, etc).
