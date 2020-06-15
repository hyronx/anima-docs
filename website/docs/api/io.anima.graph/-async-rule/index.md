[anima](../../index.md) / [io.anima.graph](../index.md) / [AsyncRule](./index.md)

# AsyncRule

`interface ~~AsyncRule~~`
**Deprecated:** Currently stick with the synchronous version

Represents a validation and customization rule for a [Graph](../-graph/index.md).

### Functions

| Name | Summary |
|---|---|
| [apply](apply.md) | Applies one or more changes to the relationships of [outVertex](apply.md#io.anima.graph.AsyncRule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/outVertex).`abstract fun apply(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)<br>`open fun apply(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, outputPromise: Promise<`[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Applies one or more changes represented by this rule to every outgoing vertex in the given [Graph](../-graph/index.md).`open fun apply(graph: `[`Graph`](../-graph/index.md)`): Future<`[`Graph`](../-graph/index.md)`>` |
| [validate](validate.md) | Validates the relationships of [outVertex](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/outVertex) represented by [edgeVertexPairs](validate.md#io.anima.graph.AsyncRule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean)/edgeVertexPairs).`abstract fun validate(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>`open fun validate(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, outputPromise: Promise<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
