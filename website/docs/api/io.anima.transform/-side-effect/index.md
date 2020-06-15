[anima](../../index.md) / [io.anima.transform](../index.md) / [SideEffect](./index.md)

# SideEffect

`interface SideEffect<A : `[`Immutable`](../-immutable/index.md)`> : `[`Transformation`](../-transformation/index.md)`<A, NoResult>`

Represents a [Transformation](../-transformation/index.md) not producing outputs but only consuming.

Use this transformation type to act upon input data like storing it somewhere without
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

### Extension Functions

| Name | Summary |
|---|---|
| [getEmptySetTransformation](../get-empty-set-transformation.md) | `fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`SideEffect`](./index.md)`<A>.getEmptySetTransformation(): `[`Transformation`](../-transformation/index.md)`<A, B>` |

### Inheritors

| Name | Summary |
|---|---|
| [GraphStoreWriteTransformation](../../io.anima.core.store/-graph-store-write-transformation/index.md) | Writes an [AnimaGraphCapsule](../-anima-graph-capsule/index.md) to the graph store with the defined [storeFormat](#)`class GraphStoreWriteTransformation : `[`SideEffect`](./index.md)`<`[`AnimaGraphCapsule`](../-anima-graph-capsule/index.md)`>` |
| [GremlinGraphSink](../../io.anima.core.transform/-gremlin-graph-sink/index.md) | Stores the input in a local Gremlin database.`class GremlinGraphSink : `[`SideEffect`](./index.md)`<`[`ExtendedAnimaGraphCapsule`](../-extended-anima-graph-capsule/index.md)`>` |
