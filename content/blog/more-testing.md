---
path: test1/tester
date: 2020-02-11T20:30:51.693Z
title: more testing
description: This is a description
---
* IPFS hosting 101 - Can my site be deployed on IPFS? - list of things that would or not work - relative vs absolute links, frameworks, tips for deploying site on IPFS, nodeJS backend, do they need to switch something for it to be able to work
* DNS - details of how the pointing works
* CDN
* Will it be fast

IPFS (interplanetary file system) is a peer to peer distributed protocol to store and access files.

Deploying a site to ipfs is easy if your site is static (ie. displaying data that is not changing).

![](assets/codesandboxBug2.png)

If you need to run a backend, it becomes more complicated.

If your site is dynamic (takes in any user input) then it becomes more complicated because all files are immutable, meaning once they are written, they cannot be changed or removed. Only a new updated version of the file can be deployed. This can be handled using ipns to set your url to the new file.

You would need to program your website specifically in preparation of deploying it to ipfs if it is not static.

IPNS - allows for the generation of a link that updates to point to the correct ipfs hash when you make updates to your website, which is effectively the same as publishing a new updated version of your website and results in a new hash. (your old version will still be published on ipfs at its original hash)
