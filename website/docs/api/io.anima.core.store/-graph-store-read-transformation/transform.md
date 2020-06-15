[anima](../../index.md) / [io.anima.core.store](../index.md) / [GraphStoreReadTransformation](index.md) / [transform](./transform.md)

# transform

`fun transform(input: `[`GraphStoreRead`](../../io.anima.core.transform/-graph-store-read.md)`, outputPromise: Promise<`[`GraphStoreCapsule`](../../io.anima.core.transform/-graph-store-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Reads the graph store.

The input is ignored. Only the input type is relevant for triggering this transformation.
It completes with a [GraphStoreCapsule](../../io.anima.core.transform/-graph-store-capsule/index.md).

### Parameters

`input` - The ignored input

`outputPromise` - The promise completing with the [GraphStoreCapsule](../../io.anima.core.transform/-graph-store-capsule/index.md)