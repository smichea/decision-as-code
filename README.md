# Decision as Code, a whitepaper


## Introduction
DAOs usually share decision power in their members through tokens and register the votes on a blockchain.
They can use the power of smart contracts to automatically trigger actions on the blockchain once a resolution is voted
but this is rarely more complex than performing coins or token transfers.
We present here a system that allow DAOs to implement complex actions automation following a decision.
Since it is very similar to IaC in its principles, we call it DaC (Decision as Code).


## From Software management to Organization management

Software have always been managed by using source code.
The code of a software is organized as files in a directory, that can have sub directories, and that we call the source code repository.
If a team share the same code repository, they can independently build the exact same version of the software.

In infrastructure management, the administrators where traditionally using interactive sessions to update the state of servers.
With the rize of coud providers and need to start and stop many servers rapidly and reliably, the administrators turned
to devops by managing the states or state change of their services in code repositories.

We believe that organizations will also benefit for using this approach where all their laws, bylaws, rules... are simply files
organized in a directory: the organization repository.  

## Versionning

Versionning system have been used for decades in software industry.
It provides a way to record all the modifications to a source code repository so you can easily restore any past state if needed.
Also it provides a way to audit a repository, wo you understand who did what and when.

In an organisation it is also very important to keep track of all versions of the rules.
If one want to understand the rationale beind a rule, it is helpful to be able to see its history and see who created or modified it in the past.


## The Git revolution
Git is a distributed source version control system created by Linus Torval in 2005.
You clone the code from somewhere, modify it, then people can clone your modified version.
This approach is adpated to the open source model where anyone can clone your code without even having to ask.
Eventually since Git also have other great features, like being able to work offline, most companies adopted git even though
they were closing their code.

In the commercial world, you get granted access to a git repository, clone its code, modify it and push back your modification.
It is like using a car solely to stay dry when it rains.
It surely does the job but if you were not scared to drive you would discover an entire new world.

This is not only its decetralized nature that makes Git well adapted to DAO needs: 
* Reliability: Git represents the state of a repository by the use of cryptographic hash (think blocks in a blockchain) 
so you can garanty that what you write once is what you read later.
* Performance: Git is a software that does not consume a lot of resources.
 

## Glossary

DAO: Decentralized Autonomous Organization.

IaC: Infrastructure as code.
