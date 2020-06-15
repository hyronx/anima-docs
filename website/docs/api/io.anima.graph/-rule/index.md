[anima](../../index.md) / [io.anima.graph](../index.md) / [Rule](./index.md)

# Rule

`interface Rule : `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

Represents a validation and customization rule for a [Graph](../-graph/index.md).

### Functions

| Name | Summary |
|---|---|
| [apply](apply.md) | Applies one or more changes to the relationships of [outVertex](apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex).`abstract fun apply(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, graph: `[`Graph`](../-graph/index.md)`): `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)<br>Applies one or more changes represented by this rule to every outgoing vertex in the given [Graph](../-graph/index.md).`open fun apply(graph: `[`Graph`](../-graph/index.md)`): `[`Graph`](../-graph/index.md) |
| [validate](validate.md) | Validates the relationships of [outVertex](validate.md#io.anima.graph.Rule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex) represented by [edgeVertexPairs](validate.md#io.anima.graph.Rule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/edgeVertexPairs).`abstract fun validate(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, graph: `[`Graph`](../-graph/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [ApplyTagRule](../../io.anima.rules/-apply-tag-rule/index.md) | `class ApplyTagRule : `[`Rule`](./index.md) |
