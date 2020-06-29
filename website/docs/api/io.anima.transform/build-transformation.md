[anima](../index.md) / [io.anima.transform](index.md) / [buildTransformation](./build-transformation.md)

# buildTransformation

`fun <A : `[`Immutable`](-immutable/index.md)`, B : `[`Immutable`](-immutable/index.md)`> buildTransformation(transformationName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, builder: `[`TransformationBuilder`](-transformation-builder/index.md)`<A, B>.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Transformation`](-transformation/index.md)`<A, B>`

Creates a new transformation with [builder](build-transformation.md#io.anima.transform$buildTransformation(kotlin.String, java.lang.Class((io.anima.transform.buildTransformation.A)), java.lang.Class((io.anima.transform.buildTransformation.B)), kotlin.Function1((io.anima.transform.TransformationBuilder((io.anima.transform.buildTransformation.A, io.anima.transform.buildTransformation.B)), kotlin.Unit)))/builder).

This method should be used for simpler transformations. If you require multiple methods,
stick with the usual way of subclassing [Transformation](-transformation/index.md).

### Parameters

`transformationName` - The name for the transformation as seen in logs

`builder` - The builder for configuring the transformation

**Return**
The registered [Transformation](-transformation/index.md)

