---
id: knowledge
title: Chapter 3: Knowledge
---

## The Basics

Knowledge in Anima is stored in a graph as described
in the [previous parts](/docs/components). It could be any data modelled by
vertices and edges. Inside the graph these building blocks can be loosely
categorized into actual objects with attributes and types defining of which
kind these objects are. There is also metadata attached to every edge that
provides information about e.g. the creator and the time of creation of one
particular edge. You can read more about it [here](/docs/graph).

On a higher level all data can be summarized to be a set of information.
In Anima each information given by an edge and its two connected vertices
has to fulfill a number of simple criteria. It must have a creator and a
creation time, which will be covered in the [next chapter](/docs/identities),
to be approved. Beside this, there exists a special subset.

## The Core knowledge

Information in this subset must be provable. This means every node must
have a Meta-edge called [_proven-by_](/docs/graph#proven-by) assigned to it.
The proof this links to must be sound and complete
for the whole **Core** knowledge. Otherwise it will be rejected.

The process of proving is done by the Minds which usually utilize Nerves
specialized for this task. They may and should use different algorithms
to improve the reliability of the proof's result. The three quarter of
the whole network need to approve the addition to get accepted
as **Core** knowledge by the network. More information about this process can
be found [here](/docs/consensus).

So called reasoners which are [Nerves](/docs/components#nerves), try to find
implicit knowledge and make it explicit through a set of rules.
Every discovery they achieve must be provable and accepted by the network as well.

If proving fails and after removing the _proven-by_ relation from an unprovable edge
it can still be added to the graph as **Mantle** knowledge.

## The Mantle knowledge

**Mantle** knowledge includes all accepted information
which is not **Core** knowledge. It is based on assumptions and may represent or
be driven by opinions. Users in Anima can vote for edges
which may semantically contradict with one or more other edges.
Agents like bots or frontends can use this information
to order answers to questions that involve **Mantle** knowledge or use it for
further processing. Such processed data cannot be assumed to be correct but
only to be sound and complete by a certain probability which must be shown to
the requesting user.

Knowledge in this layer will be analyzed by reasoners which are Nerves
responsible for extending the **Core** knowledge. They try to find proof by
semantically following the edges of high voted data back to **Core** edges
if such

## The Sphere knowledge

This is knowledge on the "edges" of the graph. Here you will find private,
mostly encrypted data like files or [identities](/docs/identities).
Like **Mantle** knowledge data being part of this layer must have
the minimum metadata like creator and creation date assigned to it.
No votes on private edges are possible nor required because the owner has full
control about it and its meaningfulness. The owner which or who is the creator
in the first place can tell Nerves like reasoners to consider his data for
private research. The person or agent can also decide to make some of its knowledge
publicly available for read-only access or even bring it into the **Mantle** layer.
In that case it looses its governing control over the data and becomes
a common, voting user of it like every other identity in Anima.

## About the names

The names (**Core**, **Mantle**, **Sphere**) follow an imagination in
which all knowledge is build and connected like in a planet
where each layer lies above and relies upon the one below it.

![Example core/sphere image](https://preview.free3d.com/img/2013/02/2206026421657143178/0bh29ash-900.jpg)
_How to imagine knowledge in Anima_
