---
id: graph
title: Graph Design
---

## The Graph Design

In Anima the graph consists of three basic categories:

* Real
* Abstract
* Meta

The **Real** vertices are instances of some classified object or type.
If you have a background in programming you can see them as the concrete objects.

Vertices of the **Abstract** category define the corresponding type hierarchy and connect each vertex
in the Real part to at least one type through the *instance-of* edge.
More about the different edge types can be found [here](#Edge-types).

To actually define these edge types the **Meta** category exists. It specifies what a *vertex* and an *edge*
is. By doing so it is possible to extend these definitions with required or optional properties.
For example, every **edge** has a **Meta-edge** called *tagged* which assigns a tag to this edge and categorize
it semantically. Another example is the *created-at* Meta-edge which specifies when an edge has been added to
the graph.

The **Real** and **Abstract** categories aren't totally hardcoded and
may sometimes overlap for some edges. You can imagine them as living in
a two dimensional grid while the **Meta** edges exist in a third dimension.

### Edge types

The following information should help you understand this edge type documentation.

Some types have one or more examples given. These examples follow the [Cypher](https://www.opencypher.org/)
graph query language loosely. In most cases it's enough to understand that vertices are defined
as **(\<vertex-name\>)** (in parentheses) and edges as **\[\<edge-name\>\]** with a directed
arrow in between them.

In general an edge has a starting vertex which we refer to as the **out-vertex** because
the edge leaves it. The ending vertex is then called the **in-vertex** because the edge ends in it.

Edges can span over one or two categories. To express this you will either find a category stated or a statement
of the pattern: *\<from-category\>* -> *\<to-category\>*.

Some times you will discover notes talking about *rules*. [Minds](/components#Mind) use them to automatically shape
the graph as desired. They must follow the rules of logic and the consensus of the network for
their changes to get accepted.

#### instance-of

**Definition**:
Defines that the out-vertex is an instance of the in-vertex.

**Examples**:

![(1)-\[instance-of\]->(number)](/img/anima_edge_instance-of.png)

**Notes**:
* Rule should use these edges to check the instance's integrity as defined by the type (the in-vertex).

**Categories**:
* Real -> Abstract
* Abstract -> Meta

#### same-as

**Definition**:
Defines that the out-vertex is identical to the in-vertex.

**Examples**:

![(1)-\[same-as\]->(1)](/img/anima_edge_same-as.png)

**Notes**:
* If such an edge is discovered, a rule might want to remove one of the connected vertices.

**Categories**:
* Real
* Abstract
* Meta
* Real -> Abstract
* Abstract -> Meta

#### equal

**Definition**:
Defines that the out-vertex is semantically equal to the in-vertex. In other words
the in-vertex means the same thing as the out-vertex but uses a different symbol for it.

**Examples**:

![(1)-\[equals\]->(one)](/img/anima_edge_equals.png)

**Notes**:
* A rule might use this edge to infer type equality.

**Categories**:
* Real
* Abstract
* Meta
* Real -> Abstract
* Abstract -> Meta

#### tagged

**Definition**:
Puts a tag on an edge for categorization. This is a Meta-edge.

**Examples**:

![(1)-\[tagged\]->(mathematics)](/img/anima_edge_tagged.png)

**Categories**:
* Real
* Abstract
* Meta

#### proven-by

**Definition**:
Points to proof of this edge. This is a Meta-edge.

**Examples**:

![(1)-\[succeeded-by\]->(2)](/img/anima_edge_proven-by.png)

**Categories**:
* Real
* Abstract
* Meta
