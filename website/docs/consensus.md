---
id: consensus
title: Chapter 4: Consensus
---

## The Basics

Knowledge is added to the Anima graph by creating a transaction, signing it and
send it to the provers for approval. A transaction contains all vertices and
edges which are requested to be added, modified or removed from the graph. Also
all required metadata must be assigned to the edges. Sending and processing
a transaction costs a fee. Otherwise provers would probably go on strike and
the network would be flooded with requests for approval.

Accepted transactions are collected to build a block of a certain size which
is then added to a [blockchain](https://en.wikipedia.org/wiki/Blockchain)
with the help and power of [Hyperledger](https://www.hyperledger.org/).

We are still figuring out the details, so expect some rough edges.
More information and deeper insides about this topic will come soon.

## When is consensus required?

Consensus is required for the acceptance of knowledge in each of the previously
described layers. About their requirements can be read
[here](/docs/knowledge) again. As you will learn in the next chapter, also
files and identities are data which must be accepted by the whole network to
be redundantly and world-wide accessibly stored. But don't worry, they belong
to the private **Sphere** layer, so as long as you are the creator you claim
to be, no data will be rejected.

## How is consensus achieved?

Consensus is achieved by utilizing the blockchain. Provers have to simply give a go
or no-go based on their discovery for the next block to be generated.
If the great majority of 75 percent agrees on acceptance, the block and its
included transactions are added to the blockchain. At our current development
and research level we don't know if it is necessary to create a new proof
algorithm or if we can probably reuse
the [Proof of Stake](https://en.wikipedia.org/wiki/Proof_of_stake) in some way.

## How do provers know if the transaction is acceptable?

For the creator proof, the _created-by_ Meta-edge will point to a public
certificate of the claimed creator. If the changes to the graph signed by
the private certificate of the creator matches and other criteria is fulfilled
the transaction will be accepted for **Mantle** and **Sphere** knowledge.

For **Core** knowledge, the requirements of sound and completeness must be
met for every edge with its _proven-by_ relationship for the whole **Core** layer.
