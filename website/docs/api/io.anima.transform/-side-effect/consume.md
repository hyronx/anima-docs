[anima](../../index.md) / [io.anima.transform](../index.md) / [SideEffect](index.md) / [consume](./consume.md)

# consume

`abstract fun consume(input: A, finishPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Consumes the input and returns nothing.

Override this method when implementing this [SideEffect](index.md).

### Parameters

`input` - The input to consume

`finishPromise` - The promise to complete when finished consuming

**See Also**

[Transformation.transform](../-transformation/transform.md)

