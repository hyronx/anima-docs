[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](index.md) / [getTree](./get-tree.md)

# getTree

`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> getTree(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>): `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>`

Gets a transformation tree without invoking it.

You can use this method to operate on the tree before invoking it.

`fun <reified A : `[`Immutable`](../-immutable/index.md)`, reified B : `[`Immutable`](../-immutable/index.md)`> getTree(): `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>`

Gets a transformation tree without invoking it.

This is the inline reified version of [getTree](./get-tree.md).

