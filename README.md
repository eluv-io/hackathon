# Eluvio Hackathon Instructions

### Welcome!

Eluvio is thrilled to be part of this great Hackathon, and to work with all of you on great solutions to our API challenge.

The Eluvio Content Fabric is a work-in-progress, novel decentralized platform for managing, distributing, selling and enjoying digital content over the Internet. Built for media from the ground up, it makes developing and deploying rich media applications very easy.

The platform combines together several new technologies we've built from scratch: Fast, machine learning driven content routing and low-latency media streaming; Decentralized storage of media and metadata without duplication; Programmable, just-in time composition; Trustless content protection from creator to consumer; Ethereum-compatible blockchain-controlled content access; Smart contracts for multi-party transactions.

### Developing a Content Fabric Application

A Content Fabric application consists of:

(a) The content 'bitcode' - this is code that operates on the content itself and is published into the fabric. This is C/C++ code compiled into LLVM bitcode. It will be executed by any fabric node as necessary (for example code that creates a 10 second trailer from a video clip, adds overlays or interactive controls, puts glasses and mustaches on characters or counts the number of key frames) 

(b) The smart contract (Ethereum Solidity) which implements the logic that allows uses to access the content, pay or get paid, etc 

(c) The front end application which uses the content fabric API as a backend (no other backend necessary unless specifically desired)

###  Challenge Details

Create a Content Fabric application that utilizes all three categories of code - bitcode, smart contracts, front end - and has at least two type of users (for example content owners, consumers, advertisers, publishers, service providers, etc).

The Content Fabric is perfectly suitable for developing your very own Spotify or Youtube, but in the same time we are more excited to learn of new kinds of applications you might think of (in the entertainment space but also any other area that can benefit from rich media and built-in commerce).

### Where to start

The best place to start is the API introduction: https://github.com/eluv-io/hakckathon/wiki/API-Quick-Start-for-the-Content-Fabric-APIs

Quicklinks:

JavaScript client API documentation: https://eluv-io.github.io/elv-client-js/ElvClient.html

Programmable media (bitcode deployed into the fabric): [https://github.com/eluv-io/content-bitcode](https://github.com/eluv-io/content-bitcode)



