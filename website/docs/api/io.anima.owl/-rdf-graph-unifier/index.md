[anima](../../index.md) / [io.anima.owl](../index.md) / [RdfGraphUnifier](./index.md)

# RdfGraphUnifier

`class RdfGraphUnifier : `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`RdfGraph`](../-rdf-graph/index.md)`, `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>`

Transforms a RDF graph to an Anima graph.

Transformation: [RdfGraph](../-rdf-graph/index.md) -&gt; [AnimaGraphCapsule](../../io.anima.transform/-anima-graph-capsule/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Transforms a RDF graph to an Anima graph.`RdfGraphUnifier()` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | `val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`RdfGraph`](../-rdf-graph/index.md)`>` |
| [outputType](output-type.md) | `val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [transform](transform.md) | `fun transform(input: `[`RdfGraph`](../-rdf-graph/index.md)`, outputPromise: Promise<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
