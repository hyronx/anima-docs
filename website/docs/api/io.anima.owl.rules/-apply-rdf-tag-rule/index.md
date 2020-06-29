[anima](../../index.md) / [io.anima.owl.rules](../index.md) / [ApplyRdfTagRule](./index.md)

# ApplyRdfTagRule

`class ApplyRdfTagRule : `[`Rule`](../../io.anima.graph/-rule/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `ApplyRdfTagRule()` |

### Functions

| Name | Summary |
|---|---|
| [apply](apply.md) | Applies one or more changes to the relationships of [outVertex](../../io.anima.graph/-rule/apply.md#io.anima.graph.Rule$apply(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex).`fun apply(outVertex: `[`Vertex`](../../io.anima.graph/-vertex/index.md)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)`, graph: `[`Graph`](../../io.anima.graph/-graph/index.md)`): `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md) |
| [filter](filter.md) | Decides whether to transform or not.`fun filter(input: `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, context: `[`TransformationContext`](../../io.anima.transform/-transformation-context/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [validate](validate.md) | Validates the relationships of [outVertex](../../io.anima.graph/-rule/validate.md#io.anima.graph.Rule$validate(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/outVertex) represented by [edgeVertexPairs](../../io.anima.graph/-rule/validate.md#io.anima.graph.Rule$validate(io.anima.graph.Vertex, kotlin.collections.Set((kotlin.Pair((io.anima.graph.Edge, io.anima.graph.Vertex)))), io.anima.graph.Graph)/edgeVertexPairs).`fun validate(outVertex: `[`Vertex`](../../io.anima.graph/-vertex/index.md)`, edgeVertexPairs: `[`EdgeToInVertexPairs`](../../io.anima.graph/-edge-to-in-vertex-pairs.md)`, graph: `[`Graph`](../../io.anima.graph/-graph/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
