[anima](../../index.md) / [io.anima.graph](../index.md) / [AsyncRule](index.md) / [apply](./apply.md)

# apply

`abstract fun apply(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)

Applies one or more changes to the relationships of [outVertex](apply.md#io.anima.graph.AsyncRule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/outVertex).

This method is synchronous version of [apply](./apply.md).
If something goes wrong, throw a custom exception.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`isMeta` - Implies whether or not [outVertex](apply.md#io.anima.graph.AsyncRule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/outVertex) and [edgeVertexPairs](apply.md#io.anima.graph.AsyncRule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/edgeVertexPairs) are meta data`open fun apply(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, outputPromise: Promise<`[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Applies one or more changes to the relationships of [outVertex](apply.md#io.anima.graph.AsyncRule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.vertx.core.Promise((kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))))))/outVertex).

If something goes wrong, throw a custom exception.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`isMeta` - Implies whether or not [outVertex](apply.md#io.anima.graph.AsyncRule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.vertx.core.Promise((kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))))))/outVertex) and [edgeVertexPairs](apply.md#io.anima.graph.AsyncRule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.vertx.core.Promise((kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))))))/edgeVertexPairs) are meta data

`outputPromise` - A promise returning the changed pairs or an exception`open fun apply(graph: `[`Graph`](../-graph/index.md)`): Future<`[`Graph`](../-graph/index.md)`>`

Applies one or more changes represented by this rule to every outgoing vertex in the given [Graph](../-graph/index.md).

### Parameters

`graph` - The graph to apply this rule to

**Return**
A future with a copy of [graph](apply.md#io.anima.graph.AsyncRule$apply(io.anima.graph.Graph)/graph) with the applied changes

