[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](index.md) / [filter](./filter.md)

# filter

`open fun filter(input: A, context: `[`TransformationContext`](../-transformation-context/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)

Decides whether to transform or not.

You can use this method to filter out some input which
this transformation doesn't support without stopping
the whole transformation process.

### Parameters

`input` - The input to filter

**Return**
True if [transform](transform.md) should be applied otherwise false

