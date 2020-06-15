[anima](../../index.md) / [io.anima.core.transform](../index.md) / [GremlinGraphSink](./index.md)

# GremlinGraphSink

`class GremlinGraphSink : `[`SideEffect`](../../io.anima.transform/-side-effect/index.md)`<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>`

Stores the input in a local Gremlin database.

This transformation is a side effect but can explicitly be addressed by creating it with [createAddressable](create-addressable.md).

### Types

| Name | Summary |
|---|---|
| [Explicit](-explicit.md) | `object Explicit : `[`Immutable`](../../io.anima.transform/-immutable/index.md) |

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Stores the input in a local Gremlin database.`GremlinGraphSink(traversalSource: SparqlTraversalSource)` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | `val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [consume](consume.md) | `fun consume(input: `[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`, finishPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | Creates an instance of [GremlinGraphSink](./index.md) as a side effect transformation.`fun create(traversalSource: SparqlTraversalSource): `[`GremlinGraphSink`](./index.md) |
| [createAddressable](create-addressable.md) | Creates an instance of [GremlinGraphSink](./index.md) as a transformation returning [Explicit](-explicit.md).`fun createAddressable(traversalSource: SparqlTraversalSource): `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`, Explicit>` |

### Extension Functions

| Name | Summary |
|---|---|
| [getEmptySetTransformation](../../io.anima.transform/get-empty-set-transformation.md) | `fun <A : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`, B : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`> `[`SideEffect`](../../io.anima.transform/-side-effect/index.md)`<A>.getEmptySetTransformation(): `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<A, B>` |
