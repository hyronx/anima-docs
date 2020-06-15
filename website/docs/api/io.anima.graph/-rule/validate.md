[anima](../../index.md) / [io.anima.graph](../index.md) / [Rule](index.md) / [validate](./validate.md)

# validate

`abstract fun validate(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, graph: `[`Graph`](../-graph/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)

Validates the relationships of [outVertex](validate.md#io.anima.graph.Rule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex) represented by [edgeVertexPairs](validate.md#io.anima.graph.Rule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/edgeVertexPairs).

This method is the synchronous version of [validate](./validate.md) and
should return true if the input is correct or false otherwise.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`isMeta` - Implies whether or not [outVertex](validate.md#io.anima.graph.Rule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex) and [edgeVertexPairs](validate.md#io.anima.graph.Rule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/edgeVertexPairs) are meta data

`graph` - The whole graph

**Return**
True if the input is correct or false otherwise

