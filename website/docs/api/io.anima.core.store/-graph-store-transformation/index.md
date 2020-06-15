[anima](../../index.md) / [io.anima.core.store](../index.md) / [GraphStoreTransformation](./index.md)

# GraphStoreTransformation

`class GraphStoreTransformation : `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`, `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>`

Transforms a graph store to a general Anima graph.

Transformation: [GraphStoreCapsule](../../io.anima.core.transform/-graph-store-capsule/index.md) -&gt; [AnimaGraphCapsule](../../io.anima.transform/-anima-graph-capsule/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Transforms a graph store to a general Anima graph.`GraphStoreTransformation()` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | `val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`>` |
| [outputType](output-type.md) | `val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [transform](transform.md) | `fun transform(input: `[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`, outputPromise: Promise<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
