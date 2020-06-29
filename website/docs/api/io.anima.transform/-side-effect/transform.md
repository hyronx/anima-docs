[anima](../../index.md) / [io.anima.transform](../index.md) / [SideEffect](index.md) / [transform](./transform.md)

# transform

`open fun transform(input: A, outputPromise: Promise<NoResult>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Transforms the input to [NoResult](-no-result.md).

This is necessary because the transformation system always requires results.
To ease the implementation, override [consume](consume.md).

**See Also**

[Transformation.invoke](../-transformation/invoke.md)

