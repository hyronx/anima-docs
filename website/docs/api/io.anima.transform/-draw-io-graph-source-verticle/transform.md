[anima](../../index.md) / [io.anima.transform](../index.md) / [DrawIoGraphSourceVerticle](index.md) / [transform](./transform.md)

# transform

`fun transform(input: `[`DrawIoInput`](../-draw-io-input/index.md)`, outputPromise: Promise<`[`DrawIoGraphCapsule`](../-draw-io-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Transforms the input to some output.

This method must be implemented as a pure function.
This method only gets [DEFAULT_TIMEOUT](../-transformation/-d-e-f-a-u-l-t_-t-i-m-e-o-u-t.md) milliseconds for completion.
If you need more, you can disable the timeout by overriding [enableTimeout](../-transformation/enable-timeout.md).

### Parameters

`input` - The input

`outputPromise` - A promise returning the output or an error

**Return**
Unit because the result is returned by [outputPromise](../-transformation/transform.md#io.anima.transform.Transformation$transform(io.anima.transform.Transformation.A, io.vertx.core.Promise((io.anima.transform.Transformation.B)))/outputPromise)

