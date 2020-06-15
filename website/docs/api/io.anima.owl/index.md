[anima](../index.md) / [io.anima.owl](./index.md)

## Package io.anima.owl

### Types

| Name | Summary |
|---|---|
| [OwlMainVerticle](-owl-main-verticle/index.md) | `class OwlMainVerticle : `[`AnimaVerticle`](../io.anima/-anima-verticle/index.md) |
| [RdfGraph](-rdf-graph/index.md) | `data class RdfGraph : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [RdfGraphUnifier](-rdf-graph-unifier/index.md) | Transforms a RDF graph to an Anima graph.`class RdfGraphUnifier : `[`Transformation`](../io.anima.transform/-transformation/index.md)`<`[`RdfGraph`](-rdf-graph/index.md)`, `[`AnimaGraphCapsule`](../io.anima.transform/-anima-graph-capsule/index.md)`>` |
| [RdfInput](-rdf-input/index.md) | `sealed class RdfInput : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [RdfTurtleInput](-rdf-turtle-input/index.md) | `data class RdfTurtleInput : `[`RdfInput`](-rdf-input/index.md) |
| [RdfTurtleTransformation](-rdf-turtle-transformation/index.md) | Transforms a RDF Turtle input to a RDF graph.`class RdfTurtleTransformation : `[`Transformation`](../io.anima.transform/-transformation/index.md)`<`[`RdfTurtleInput`](-rdf-turtle-input/index.md)`, `[`RdfGraph`](-rdf-graph/index.md)`>` |
| [RdfXmlInput](-rdf-xml-input/index.md) | `data class RdfXmlInput : `[`RdfInput`](-rdf-input/index.md) |
| [RdfXmlTransformation](-rdf-xml-transformation/index.md) | Transforms a RDF XML input to a RDF graph.`class RdfXmlTransformation : `[`Transformation`](../io.anima.transform/-transformation/index.md)`<`[`RdfXmlInput`](-rdf-xml-input/index.md)`, `[`RdfGraph`](-rdf-graph/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [transform](transform.md) | Transforms the RDF input to a RDF graph.`fun transform(lang: Lang, logger: Logger, input: `[`RdfInput`](-rdf-input/index.md)`, outputPromise: Promise<`[`RdfGraph`](-rdf-graph/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
