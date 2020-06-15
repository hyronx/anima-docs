[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationTree](index.md) / [create](./create.md)

# create

`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> create(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>): `[`TransformationTree`](index.md)`<A, B>`

Creates a new [TransformationTree](index.md).

You doesn't usually invoke this method directly but instead call [TransformationTreeBuilder.build](../-transformation-tree-builder/build.md).

### Parameters

`inputType` - The input type

`outputType` - The output type`fun <reified A : `[`Immutable`](../-immutable/index.md)`, reified B : `[`Immutable`](../-immutable/index.md)`> create(vertx: Vertx): `[`TransformationTree`](index.md)`<A, B>`

Creates a new [TransformationTree](index.md).

You doesn't usually invoke this method directly but instead call [TransformationTreeBuilder.build](../-transformation-tree-builder/build.md).

