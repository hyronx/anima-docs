[anima](../../index.md) / [io.anima.rules](../index.md) / [ApplyTagRule](index.md) / [apply](./apply.md)

# apply

`fun apply(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, graph: `[`Graph`](../../io.anima.graph/-graph/index.md)`): `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)

Applies one or more changes to the relationships of [outVertex](../../io.anima.graph/-rule/apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex).

This method is synchronous version of [apply](../../io.anima.graph/-rule/apply.md).
If something goes wrong, throw a custom exception.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`isMeta` - Implies whether or not [outVertex](../../io.anima.graph/-rule/apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex) and [edgeVertexPairs](../../io.anima.graph/-rule/apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/edgeVertexPairs) are meta data

`graph` - The whole graph

**Return**
The modified edges and in-vertices for the input [outVertex](../../io.anima.graph/-rule/apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex)

