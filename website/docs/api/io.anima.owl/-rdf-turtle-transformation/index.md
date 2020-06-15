[anima](../../index.md) / [io.anima.owl](../index.md) / [RdfTurtleTransformation](./index.md)

# RdfTurtleTransformation

`class RdfTurtleTransformation : `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`RdfTurtleInput`](../-rdf-turtle-input/index.md)`, `[`RdfGraph`](../-rdf-graph/index.md)`>`

Transforms a RDF Turtle input to a RDF graph.

Transformation: [RdfTurtleInput](../-rdf-turtle-input/index.md) -&gt; [RdfGraph](../-rdf-graph/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Transforms a RDF Turtle input to a RDF graph.`RdfTurtleTransformation()` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | `val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`RdfTurtleInput`](../-rdf-turtle-input/index.md)`>` |
| [outputType](output-type.md) | `val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`RdfGraph`](../-rdf-graph/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [transform](transform.md) | Transforms the input as [Lang.TURTLE](#) using [transform](transform.md).`fun transform(input: `[`RdfTurtleInput`](../-rdf-turtle-input/index.md)`, outputPromise: Promise<`[`RdfGraph`](../-rdf-graph/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
