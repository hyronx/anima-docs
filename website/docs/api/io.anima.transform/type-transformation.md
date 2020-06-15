[anima](../index.md) / [io.anima.transform](index.md) / [typeTransformation](./type-transformation.md)

# typeTransformation

`inline fun <reified A : `[`Immutable`](-immutable/index.md)`, reified B : `[`Immutable`](-immutable/index.md)`> typeTransformation(transformationName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, crossinline transformer: (A) -> B): `[`Transformation`](-transformation/index.md)`<A, B>`

Creates a new type conversion focused transformation.

This method should only be used for one-liner type conversions.

### Parameters

`transformationName` - The name for the transformation as seen in logs

`transformer` - The handler transforming [A](type-transformation.md#A) to [B](type-transformation.md#B)

**See Also**

[buildTransformation](build-transformation.md)

**Return**
The registered [Transformation](-transformation/index.md)

