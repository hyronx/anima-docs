[anima](../../index.md) / [io.anima.core.store](../index.md) / [GraphStoreWriteTransformation](./index.md)

# GraphStoreWriteTransformation

`class GraphStoreWriteTransformation : `[`SideEffect`](../../io.anima.transform/-side-effect/index.md)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>`

Writes an [AnimaGraphCapsule](../../io.anima.transform/-anima-graph-capsule/index.md) to the graph store with the defined [storeFormat](#)

Transformation: [AnimaGraphCapsule](../../io.anima.transform/-anima-graph-capsule/index.md) -&gt; ()

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | `val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [consume](consume.md) | Write the input graph to the graph store`fun consume(input: `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, finishPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [filter](filter.md) | Decides whether to transform or not.`fun filter(input: `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, context: `[`TransformationContext`](../../io.anima.transform/-transformation-context/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun create(vertx: Vertx, storeFormat: Format, storeDirectory: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`GraphStoreWriteTransformation`](./index.md) |

### Extension Functions

| Name | Summary |
|---|---|
| [getEmptySetTransformation](../../io.anima.transform/get-empty-set-transformation.md) | `fun <A : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`, B : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`> `[`SideEffect`](../../io.anima.transform/-side-effect/index.md)`<A>.getEmptySetTransformation(): `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<A, B>` |
