[anima](../../index.md) / [io.anima.rules](../index.md) / [AddTimestampRule](index.md) / [apply](./apply.md)

# apply

`fun apply(outVertex: `[`Vertex`](../../io.anima.graph/-vertex/index.md)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)`, graph: `[`Graph`](../../io.anima.graph/-graph/index.md)`): `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)

Applies one or more changes to the relationships of [outVertex](../../io.anima.graph/-rule/apply.md#io.anima.graph.Rule$apply(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex).

This method is synchronous version of [apply](../../io.anima.graph/-rule/apply.md).
If something goes wrong, throw a custom exception.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`graph` - The whole graph

**Return**
The modified edges and in-vertices for the input [outVertex](../../io.anima.graph/-rule/apply.md#io.anima.graph.Rule$apply(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex)

