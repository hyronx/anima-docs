[anima](../../index.md) / [io.anima.rules](../index.md) / [ApplyTagRule](./index.md)

# ApplyTagRule

`class ApplyTagRule : `[`Rule`](../../io.anima.graph/-rule/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `ApplyTagRule()` |

### Functions

| Name | Summary |
|---|---|
| [apply](apply.md) | Applies one or more changes to the relationships of [outVertex](../../io.anima.graph/-rule/apply.md#io.anima.graph.Rule$apply(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex).`fun apply(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, graph: `[`Graph`](../../io.anima.graph/-graph/index.md)`): `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md) |
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`fun toJsonObject(): JsonObject` |
| [validate](validate.md) | Validates the relationships of [outVertex](../../io.anima.graph/-rule/validate.md#io.anima.graph.Rule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/outVertex) represented by [edgeVertexPairs](../../io.anima.graph/-rule/validate.md#io.anima.graph.Rule$validate(java.io.Serializable, kotlin.collections.Set((kotlin.Pair((java.io.Serializable, )))), kotlin.Boolean, io.anima.graph.Graph)/edgeVertexPairs).`fun validate(outVertex: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)`, isMeta: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`, graph: `[`Graph`](../../io.anima.graph/-graph/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
