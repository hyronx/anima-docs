[anima](../../index.md) / [io.anima.graph](../index.md) / [Rule](index.md) / [apply](./apply.md)

# apply

`abstract fun apply(outVertex: `[`Vertex`](../-vertex/index.md)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, graph: `[`Graph`](../-graph/index.md)`): `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)

Applies one or more changes to the relationships of [outVertex](apply.md#io.anima.graph.Rule$apply(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex).

This method is synchronous version of [apply](./apply.md).
If something goes wrong, throw a custom exception.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`graph` - The whole graph

**Return**
The modified edges and in-vertices for the input [outVertex](apply.md#io.anima.graph.Rule$apply(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex)

`open fun apply(graph: `[`Graph`](../-graph/index.md)`): `[`Graph`](../-graph/index.md)

Applies one or more changes represented by this rule to every outgoing vertex in the given [Graph](../-graph/index.md).

### Parameters

`graph` - The graph to apply this rule to

**Return**
A future with a copy of [graph](apply.md#io.anima.graph.Rule$apply(io.anima.graph.Graph)/graph) with the applied changes

