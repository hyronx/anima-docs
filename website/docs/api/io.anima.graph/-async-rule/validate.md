[anima](../../index.md) / [io.anima.graph](../index.md) / [AsyncRule](index.md) / [validate](./validate.md)

# validate

`abstract fun validate(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)

Validates the relationships of [outVertex](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/outVertex) represented by [edgeVertexPairs](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/edgeVertexPairs).

This method is the synchronous version of [validate](./validate.md) and
should return true if the input is correct or false otherwise.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`isMeta` - Implies whether or not [outVertex](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/outVertex) and [edgeVertexPairs](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/edgeVertexPairs) are meta data

`outputPromise` - A promise returning the validation result or an exception

**Return**
True if the input is correct or false otherwise

`open fun validate(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, outputPromise: Promise<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Validates the relationships of [outVertex](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.vertx.core.Promise((kotlin.Boolean)))/outVertex) represented by [edgeVertexPairs](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.vertx.core.Promise((kotlin.Boolean)))/edgeVertexPairs).

This method should return true using [outputPromise](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.vertx.core.Promise((kotlin.Boolean)))/outputPromise) if the input is correct or false otherwise.

### Parameters

`outVertex` - The vertex where the edges start

`edgeVertexPairs` - The edges and the vertices they end up in

`isMeta` - Implies whether or not [outVertex](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.vertx.core.Promise((kotlin.Boolean)))/outVertex) and [edgeVertexPairs](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.vertx.core.Promise((kotlin.Boolean)))/edgeVertexPairs) are meta data

`outputPromise` - A promise returning the validation result or an exception

**Return**
True if the input is correct or false otherwise

