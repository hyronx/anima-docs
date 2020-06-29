[anima](../../index.md) / [io.anima.graph](../index.md) / [Rule](./index.md)

# Rule

`interface Rule : `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, `[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>`

Represents a validation and customization rule for a [Graph](../-graph/index.md).

This interface is a more specific transformation. Because it is still used
as a [Transformation](../../io.anima.transform/-transformation/index.md), you can override methods as you need. The added
[validate](validate.md) and [apply](apply.md) methods should be seen as guide lines on how to
implement and work with rules.

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | The input type for this transformation`open val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>` |
| [outputType](output-type.md) | The output type for this transformation`open val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [apply](apply.md) | Applies one or more changes to the relationships of [outVertex](apply.md#io.anima.graph.Rule$apply(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex).`abstract fun apply(outVertex: `[`Vertex`](../-vertex/index.md)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, graph: `[`Graph`](../-graph/index.md)`): `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)<br>Applies one or more changes represented by this rule to every outgoing vertex in the given [Graph](../-graph/index.md).`open fun apply(graph: `[`Graph`](../-graph/index.md)`): `[`Graph`](../-graph/index.md) |
| [transform](transform.md) | Transforms the input to some output.`open fun transform(input: `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, outputPromise: Promise<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [validate](validate.md) | Validates the relationships of [outVertex](validate.md#io.anima.graph.Rule$validate(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex) represented by [edgeVertexPairs](validate.md#io.anima.graph.Rule$validate(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/edgeVertexPairs).`abstract fun validate(outVertex: `[`Vertex`](../-vertex/index.md)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../-edge-to-in-vertex-pairs.md)`, graph: `[`Graph`](../-graph/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [AddTimestampRule](../../io.anima.rules/-add-timestamp-rule/index.md) | `class AddTimestampRule : `[`Rule`](./index.md) |
| [ApplyRdfTagRule](../../io.anima.owl.rules/-apply-rdf-tag-rule/index.md) | `class ApplyRdfTagRule : `[`Rule`](./index.md) |
| [ApplyTagRule](../../io.anima.rules/-apply-tag-rule/index.md) | `class ApplyTagRule : `[`Rule`](./index.md) |
