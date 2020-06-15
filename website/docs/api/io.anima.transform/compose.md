[anima](../index.md) / [io.anima.transform](index.md) / [compose](./compose.md)

# compose

`fun <A : `[`Immutable`](-immutable/index.md)`, B : `[`Immutable`](-immutable/index.md)`, C : `[`Immutable`](-immutable/index.md)`> `[`TransformationTree`](-transformation-tree/index.md)`<A, B>.compose(nextOutputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<C>, outputMapper: (previousOutputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>) -> Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>> = { Future.succeededFuture(it) }): `[`TransformationTree`](-transformation-tree/index.md)`<A, C>`

Creates a new transformation tree for [A](compose.md#A) to [C](compose.md#C) by reusing this tree.

The composition is achieved by creating a new [TransformationTree](-transformation-tree/index.md)&lt;A, C&gt; and using
this tree as its first child and transformation.
The [outputMapper](compose.md#io.anima.transform$compose(io.anima.transform.TransformationTree((io.anima.transform.compose.A, io.anima.transform.compose.B)), java.lang.Class((io.anima.transform.compose.C)), kotlin.Function1((kotlin.collections.Set((io.anima.transform.compose.B)), io.vertx.core.Future(()))))/outputMapper) is called after this tree to customize its output, respectively
the next children's input.

### Parameters

`nextOutputType` - The next output type to return

`outputMapper` - A mapping function for customizing the output of this tree

**Return**
A new [TransformationTree](-transformation-tree/index.md) for [A](compose.md#A) to [C](compose.md#C)

`inline fun <A : `[`Immutable`](-immutable/index.md)`, B : `[`Immutable`](-immutable/index.md)`, reified C : `[`Immutable`](-immutable/index.md)`> `[`TransformationTree`](-transformation-tree/index.md)`<A, B>.compose(noinline outputMapper: (previousOutputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>) -> Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>> = { Future.succeededFuture(it) }): `[`TransformationTree`](-transformation-tree/index.md)`<A, C>`

Creates a new transformation tree for [A](compose.md#A) to [C](compose.md#C) by reusing this tree.

This is the inline reified version of [compose](./compose.md).

**See Also**

[compose](./compose.md)

