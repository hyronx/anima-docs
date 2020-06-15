[anima](../../index.md) / [io.anima.transform](../index.md) / [DrawIoGraphUnifierVerticle](index.md) / [transform](./transform.md)

# transform

`fun transform(input: `[`DrawIoGraphCapsule`](../-draw-io-graph-capsule/index.md)`, outputPromise: Promise<`[`AnimaGraphCapsule`](../-anima-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Transforms the input to some output.

This method must be implemented as a pure function.

### Parameters

`input` - The input

`outputPromise` - A promise returning the output or an error

**Return**
Unit because the result is returned by [outputPromise](../-transformation/transform.md#io.anima.transform.Transformation$transform(io.anima.transform.Transformation.A, io.vertx.core.Promise((io.anima.transform.Transformation.B)))/outputPromise)

