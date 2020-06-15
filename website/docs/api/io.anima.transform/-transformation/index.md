[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](./index.md)

# Transformation

`interface Transformation<A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> : (`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>, `[`TransformationContext`](../-transformation-context/index.md)`) -> Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Represents a transformation of input type [A](index.md#A) to output type [B](index.md#B).

This transformation is expected to be pure and its parameters are expected to be immutable.
This is indicated by the [Immutable](../-immutable/index.md) interface. Make sure to use as precise types as possible because
these are used for building transformation trees.

A transformation can also be passed to any method expecting a function with a set of inputs
and returning a future set of results.

Every transformation sends status messages before and after the transformation happened and might send
status messages during the process. To receive these messages create a new [TransformationStatusAddress](../-transformation-status-address/index.md)
with your input and output type. Then call [io.vertx.core.eventbus.EventBus.consumer](#) with the address
and handler for the messages. The status messages are [JsonObject](#)s. Here is an example:

```
val statusAddress = TransformationStatusAddress(SomeA::class.java, SomeB::class.java)
val consumer = vertx.eventBus().consumer<JsonObject>(statusAddress.toString()) { message ->
  // Do something with the status message
}
// When finished
consumer.unregister()
```

### Parameters

`A` - The immutable input type

`B` - The immutable output type

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | The input type for this transformation`abstract val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>` |
| [logger](logger.md) | Some logger instance which may be used in overridden methods`open val logger: Logger` |
| [name](name.md) | The name of this transformation`open val name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [outputType](output-type.md) | The output type for this transformation`abstract val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>` |

### Functions

| Name | Summary |
|---|---|
| [createStatus](create-status.md) | Creates a new status message.`open fun createStatus(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, additionalInfo: JsonObject): JsonObject!` |
| [filter](filter.md) | Decides whether to transform or not.`open fun filter(input: A, context: `[`TransformationContext`](../-transformation-context/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [invoke](invoke.md) | Calls [transform](transform.md) on an input set.`open fun invoke(inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>, context: `[`TransformationContext`](../-transformation-context/index.md)`): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`<br>Call [transform](transform.md) on an input set.`open operator fun invoke(vararg inputs: A, context: `[`TransformationContext`](../-transformation-context/index.md)`? = null): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>` |
| [publishStatus](publish-status.md) | Sends a status message.`open fun publishStatus(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, additionalInfo: JsonObject = jsonObjectOf(), deliveryOptions: DeliveryOptions = deliveryOptionsOf()): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [transform](transform.md) | Transforms the input to some output.`abstract fun transform(input: A, outputPromise: Promise<B>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>`open fun transform(input: A): Future<B!>` |

### Companion Object Functions

| Name | Summary |
|---|---|
| [getTree](get-tree.md) | Gets a transformation tree without invoking it.`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> getTree(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>): `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>`<br>`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> getTree(): `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>` |
| [init](init.md) | Initialises [vertx](init.md#io.anima.transform.Transformation.Companion$init(io.vertx.core.Vertx)/vertx).`fun init(vertx: Vertx): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [transform](transform.md) | Builds a transformation tree to transform the inputs to a set of outputs.`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> transform(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`<br>`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> transform(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`<br>`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> transform(vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>` |

### Inheritors

| Name | Summary |
|---|---|
| [GraphStoreReadTransformation](../../io.anima.core.store/-graph-store-read-transformation/index.md) | Reads the graph store with the defined [storeFormat](#)`class GraphStoreReadTransformation : `[`Transformation`](./index.md)`<`[`GraphStoreRead`](../../io.anima.core.transform/-graph-store-read.md)`, `[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`>` |
| [GraphStoreTransformation](../../io.anima.core.store/-graph-store-transformation/index.md) | Transforms a graph store to a general Anima graph.`class GraphStoreTransformation : `[`Transformation`](./index.md)`<`[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`, `[`AnimaGraphCapsule`](../-anima-graph-capsule/index.md)`>` |
| [RdfGraphUnifier](../../io.anima.owl/-rdf-graph-unifier/index.md) | Transforms a RDF graph to an Anima graph.`class RdfGraphUnifier : `[`Transformation`](./index.md)`<`[`RdfGraph`](../../io.anima.owl/-rdf-graph/index.md)`, `[`AnimaGraphCapsule`](../-anima-graph-capsule/index.md)`>` |
| [RdfTurtleTransformation](../../io.anima.owl/-rdf-turtle-transformation/index.md) | Transforms a RDF Turtle input to a RDF graph.`class RdfTurtleTransformation : `[`Transformation`](./index.md)`<`[`RdfTurtleInput`](../../io.anima.owl/-rdf-turtle-input/index.md)`, `[`RdfGraph`](../../io.anima.owl/-rdf-graph/index.md)`>` |
| [RdfXmlTransformation](../../io.anima.owl/-rdf-xml-transformation/index.md) | Transforms a RDF XML input to a RDF graph.`class RdfXmlTransformation : `[`Transformation`](./index.md)`<`[`RdfXmlInput`](../../io.anima.owl/-rdf-xml-input/index.md)`, `[`RdfGraph`](../../io.anima.owl/-rdf-graph/index.md)`>` |
| [SideEffect](../-side-effect/index.md) | Represents a [Transformation](./index.md) not producing outputs but only consuming.`interface SideEffect<A : `[`Immutable`](../-immutable/index.md)`> : `[`Transformation`](./index.md)`<A, NoResult>` |
| [SparqlQuestionMessageTransformation](../../io.anima.core.transform/-sparql-question-message-transformation/index.md) | Transforms question messages to SPARQL questions for the transformation system if possible.`class SparqlQuestionMessageTransformation : `[`Transformation`](./index.md)`<`[`QuestionMessageCapsule`](../../io.anima.core.transform/-question-message-capsule/index.md)`, `[`SparqlQuestionCapsule`](../../io.anima.core.transform/-sparql-question-capsule/index.md)`>` |
| [SparqlQuestionTransformation](../../io.anima.core.transform/-sparql-question-transformation/index.md) | `class SparqlQuestionTransformation : `[`Transformation`](./index.md)`<`[`SparqlQuestionCapsule`](../../io.anima.core.transform/-sparql-question-capsule/index.md)`, `[`SequenceAnswersCapsule`](../../io.anima.core.transform/-sequence-answers-capsule/index.md)`>` |
| [TransformationRegistrationVerticle](../-transformation-registration-verticle/index.md) | `class TransformationRegistrationVerticle<A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`, `[`Transformation`](./index.md)`<A, B>` |
| [TransformationTree](../-transformation-tree/index.md) | A tree of functions`data class TransformationTree<A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> : `[`Transformation`](./index.md)`<A, B>` |
| [TransformationVerticle](../-transformation-verticle/index.md) | `abstract class TransformationVerticle<A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`, `[`Transformation`](./index.md)`<A, B>` |
