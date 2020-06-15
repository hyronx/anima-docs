[anima](../index.md) / [io.anima.transform](index.md) / [transformation](./transformation.md)

# transformation

`fun <A : `[`Immutable`](-immutable/index.md)`, B : `[`Immutable`](-immutable/index.md)`> transformation(transformationName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, transformationHandler: (input: A, outputPromise: Promise<B>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Transformation`](-transformation/index.md)`<A, B>`

Creates a new transformation.

### Parameters

`transformationName` - The name for the transformation as seen in logs

`transformationHandler` - The handler doing the actual work for the transformation

**See Also**

[buildTransformation](build-transformation.md)

**Return**
The registered [Transformation](-transformation/index.md)

`inline fun <reified A : `[`Immutable`](-immutable/index.md)`, reified B : `[`Immutable`](-immutable/index.md)`> transformation(transformationName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, noinline transformationHandler: (input: A, outputPromise: Promise<B>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Transformation`](-transformation/index.md)`<A, B>`

Creates a new transformation.

This is the inline reified version.

### Parameters

`transformationName` - The name for the transformation as seen in logs

`transformationHandler` - The handler doing the actual work for the transformation

**See Also**

[buildTransformation](build-transformation.md)

**Return**
The registered [Transformation](-transformation/index.md)

