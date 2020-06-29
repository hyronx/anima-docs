[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](index.md) / [transform](./transform.md)

# transform

`abstract fun transform(input: A, outputPromise: Promise<B>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Transforms the input to some output.

This method must be implemented as a pure function.
This method only gets [DEFAULT_TIMEOUT](-d-e-f-a-u-l-t_-t-i-m-e-o-u-t.md) milliseconds for completion.
If you need more, you can disable the timeout by overriding [enableTimeout](enable-timeout.md).

### Parameters

`input` - The input

`outputPromise` - A promise returning the output or an error

**Return**
Unit because the result is returned by [outputPromise](transform.md#io.anima.transform.Transformation$transform(io.anima.transform.Transformation.A, io.vertx.core.Promise((io.anima.transform.Transformation.B)))/outputPromise)

`open fun transform(input: A): Future<B!>`

Transforms the input to some output.

Implement the [transform](./transform.md) method.
The [transform](./transform.md) method only gets [DEFAULT_TIMEOUT](-d-e-f-a-u-l-t_-t-i-m-e-o-u-t.md) milliseconds for completion.
If you need more, you can disable the timeout by overriding [enableTimeout](enable-timeout.md).

### Parameters

`input` - The input

**Return**
A future returning the output or an error

