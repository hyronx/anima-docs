[anima](../../index.md) / [io.anima.core.transform](../index.md) / [AnimaGraphTimestampExtender](index.md) / [transform](./transform.md)

# transform

`fun transform(input: `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, outputPromise: Promise<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Transforms the input to some output.

This method must be implemented as a pure function.

### Parameters

`input` - The input

`outputPromise` - A promise returning the output or an error

**Return**
Unit because the result is returned by [outputPromise](../../io.anima.transform/-transformation/transform.md#io.anima.transform.Transformation$transform(io.anima.transform.Transformation.A, io.vertx.core.Promise((io.anima.transform.Transformation.B)))/outputPromise)

