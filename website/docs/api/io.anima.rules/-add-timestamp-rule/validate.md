[anima](../../index.md) / [io.anima.rules](../index.md) / [AddTimestampRule](index.md) / [validate](./validate.md)

# validate

`fun validate(outVertex: `[`Vertex`](../../io.anima.graph/-vertex/index.md)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)`, graph: `[`Graph`](../../io.anima.graph/-graph/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)

Validates the relationships of [outVertex](../../io.anima.graph/-rule/validate.md#io.anima.graph.Rule$validate(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex) represented by [edgeVertexPairs](../../io.anima.graph/-rule/validate.md#io.anima.graph.Rule$validate(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/edgeVertexPairs).

This method is the synchronous version of [validate](../../io.anima.graph/-rule/validate.md) and
should return true if the input is correct or false otherwise.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`graph` - The whole graph

**Return**
True if the input is correct or false otherwise

