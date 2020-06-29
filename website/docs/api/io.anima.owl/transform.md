[anima](../index.md) / [io.anima.owl](index.md) / [transform](./transform.md)

# transform

`fun transform(lang: Lang, logger: Logger, input: `[`RdfInput`](-rdf-input.md)`, outputPromise: Promise<`[`RdfGraph`](-rdf-graph/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Transforms the RDF input to a RDF graph.

This method is used by all Rdf&lt;...&gt;Transformation classes.

### Parameters

`lang` - The domain specific language of the RDF input

`logger` - A logger instance for debug logging

`input` - The RDF input

`outputPromise` - A promise used for returning the RDF graph

**Return**
Unit because the actual result is returned by [outputPromise](transform.md#io.anima.owl$transform(org.apache.jena.riot.Lang, org.slf4j.Logger, io.anima.owl.RdfInput, io.vertx.core.Promise((io.anima.owl.RdfGraph)))/outputPromise)

