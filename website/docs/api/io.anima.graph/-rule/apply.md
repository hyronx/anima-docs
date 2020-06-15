[anima](../../index.md) / [io.anima.graph](../index.md) / [Rule](index.md) / [apply](./apply.md)

# apply

`abstract fun apply(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, graph: `[`Graph`](../-graph/index.md)`): `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)

Applies one or more changes to the relationships of [outVertex](apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex).

This method is synchronous version of [apply](./apply.md).
If something goes wrong, throw a custom exception.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`isMeta` - Implies whether or not [outVertex](apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex) and [edgeVertexPairs](apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/edgeVertexPairs) are meta data

`graph` - The whole graph

**Return**
The modified edges and in-vertices for the input [outVertex](apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex)

`open fun apply(graph: `[`Graph`](../-graph/index.md)`): `[`Graph`](../-graph/index.md)

Applies one or more changes represented by this rule to every outgoing vertex in the given [Graph](../-graph/index.md).

### Parameters

`graph` - The graph to apply this rule to

**Return**
A future with a copy of [graph](apply.md#io.anima.graph.Rule$apply(io.anima.graph.Graph)/graph) with the applied changes

