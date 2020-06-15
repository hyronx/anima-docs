[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationTreeBuilder](index.md) / [build](./build.md)

# build

`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> build(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, customBuilder: (`[`TransformationTreeBuilder`](index.md)`.(`[`TransformationTree`](../-transformation-tree/index.md)`<A, B>) -> `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>)? = null): `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>`

Builds the [TransformationTree](../-transformation-tree/index.md).

If you supply a [customBuilder](build.md#io.anima.transform.TransformationTreeBuilder$build(java.lang.Class((io.anima.transform.TransformationTreeBuilder.build.A)), java.lang.Class((io.anima.transform.TransformationTreeBuilder.build.B)), kotlin.Function2((io.anima.transform.TransformationTreeBuilder, io.anima.transform.TransformationTree((io.anima.transform.TransformationTreeBuilder.build.A, io.anima.transform.TransformationTreeBuilder.build.B)), )))/customBuilder), you still **don't** have to freeze the tree manually.

### Parameters

`inputType` - The input type

`outputType` - The output type+

`customBuilder` - A function for customizing the tree build mechanism

### Exceptions

`NoPathsFoundException` - If no paths are found for [A](build.md#A) to [B](build.md#B)

`AlreadyFrozenException` - If [customBuilder](build.md#io.anima.transform.TransformationTreeBuilder$build(java.lang.Class((io.anima.transform.TransformationTreeBuilder.build.A)), java.lang.Class((io.anima.transform.TransformationTreeBuilder.build.B)), kotlin.Function2((io.anima.transform.TransformationTreeBuilder, io.anima.transform.TransformationTree((io.anima.transform.TransformationTreeBuilder.build.A, io.anima.transform.TransformationTreeBuilder.build.B)), )))/customBuilder) returned a tree which has already been frozen

**Return**
The transformation tree instance

`inline fun <reified A : `[`Immutable`](../-immutable/index.md)`, reified B : `[`Immutable`](../-immutable/index.md)`> build(noinline customBuilder: (`[`TransformationTreeBuilder`](index.md)`.(`[`TransformationTree`](../-transformation-tree/index.md)`<A, B>) -> `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>)? = null): `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>`

Builds the [TransformationTree](../-transformation-tree/index.md).

### Parameters

`customBuilder` - A function for customizing the tree build mechanism

**See Also**

[TransformationTreeBuilder.build](./build.md)

**Return**
The transformation tree instance

