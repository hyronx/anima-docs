[anima](../../index.md) / [io.anima.owl](../index.md) / [RdfXmlTransformation](./index.md)

# RdfXmlTransformation

`class RdfXmlTransformation : `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`RdfXmlInput`](../-rdf-xml-input/index.md)`, `[`RdfGraph`](../-rdf-graph/index.md)`>`

Transforms a RDF XML input to a RDF graph.

Transformation: [RdfXmlInput](../-rdf-xml-input/index.md) -&gt; [RdfGraph](../-rdf-graph/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Transforms a RDF XML input to a RDF graph.`RdfXmlTransformation()` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | `val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`RdfXmlInput`](../-rdf-xml-input/index.md)`>` |
| [outputType](output-type.md) | `val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`RdfGraph`](../-rdf-graph/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [transform](transform.md) | Transforms the input as [Lang.RDFXML](#) using [transform](transform.md).`fun transform(input: `[`RdfXmlInput`](../-rdf-xml-input/index.md)`, outputPromise: Promise<`[`RdfGraph`](../-rdf-graph/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
