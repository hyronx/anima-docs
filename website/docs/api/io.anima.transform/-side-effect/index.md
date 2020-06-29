[anima](../../index.md) / [io.anima.transform](../index.md) / [SideEffect](./index.md)

# SideEffect

`interface SideEffect<A : `[`Immutable`](../-immutable/index.md)`> : `[`Transformation`](../-transformation/index.md)`<A, NoResult>`

Represents a [Transformation](../-transformation/index.md) not producing outputs but only consuming.

Use this transformation type to act upon input transform like storing it somewhere without
the need to return something.

### Types

| Name | Summary |
|---|---|
| [NoResult](-no-result.md) | `object NoResult : `[`Immutable`](../-immutable/index.md) |

### Properties

| Name | Summary |
|---|---|
| [outputType](output-type.md) | The output type for this transformation`open val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<NoResult>` |

### Functions

| Name | Summary |
|---|---|
| [consume](consume.md) | Consumes the input and returns nothing.`abstract fun consume(input: A, finishPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [getEmptySetTransformation](get-empty-set-transformation.md) | Creates a transformation returning an empty set of type [B](get-empty-set-transformation.md#B).`open fun <B : `[`Immutable`](../-immutable/index.md)`> getEmptySetTransformation(outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>): `[`Transformation`](../-transformation/index.md)`<A, B>` |
| [transform](transform.md) | Transforms the input to [NoResult](-no-result.md).`open fun transform(input: A, outputPromise: Promise<NoResult>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [invoke](invoke.md) | Builds a transformation tree to execute a set of side effects.`operator fun <A : `[`Immutable`](../-immutable/index.md)`> invoke(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<NoResult>>`<br>`operator fun <A : `[`Immutable`](../-immutable/index.md)`> invoke(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<NoResult>>`<br>`operator fun <A : `[`Immutable`](../-immutable/index.md)`> invoke(vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<NoResult>>` |

### Extension Functions

| Name | Summary |
|---|---|
| [getEmptySetTransformation](../get-empty-set-transformation.md) | `fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`SideEffect`](./index.md)`<A>.getEmptySetTransformation(): `[`Transformation`](../-transformation/index.md)`<A, B>` |

### Inheritors

| Name | Summary |
|---|---|
| [BridgeEventConsumer](../../io.anima.web/-bridge-event-consumer.md) | `interface BridgeEventConsumer<A : `[`IncomingEvent`](../../io.anima.web/-incoming-event/index.md)`> : `[`SideEffect`](./index.md)`<A>` |
