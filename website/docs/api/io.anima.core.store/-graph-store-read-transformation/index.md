[anima](../../index.md) / [io.anima.core.store](../index.md) / [GraphStoreReadTransformation](./index.md)

# GraphStoreReadTransformation

`class GraphStoreReadTransformation : `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`GraphStoreRead`](../../io.anima.core.transform/-graph-store-read.md)`, `[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`>`

Reads the graph store with the defined [storeFormat](#)

Transformation: [GraphStoreRead](../../io.anima.core.transform/-graph-store-read.md) -&gt; [GraphStoreCapsule](../../io.anima.core.transform/-graph-store-capsule/index.md)

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | `val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`GraphStoreRead`](../../io.anima.core.transform/-graph-store-read.md)`>` |
| [outputType](output-type.md) | `val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [transform](transform.md) | Reads the graph store.`fun transform(input: `[`GraphStoreRead`](../../io.anima.core.transform/-graph-store-read.md)`, outputPromise: Promise<`[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun create(vertx: Vertx, storeFormat: Format, storeDirectory: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`GraphStoreReadTransformation`](./index.md) |
