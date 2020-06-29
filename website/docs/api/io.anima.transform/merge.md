[anima](../index.md) / [io.anima.transform](index.md) / [merge](./merge.md)

# merge

`fun <A : `[`Immutable`](-immutable/index.md)`, B : `[`Immutable`](-immutable/index.md)`> `[`TransformationTree`](-transformation-tree/index.md)`<A, out B>.merge(baseOutputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, vararg compatibleOutputTypes: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<out B>): `[`TransformationTree`](-transformation-tree/index.md)`<A, B>`

Creates a new tree which also covers covariant types to [B](merge.md#B).

The created tree keeps the [TransformationTree.inputType](-transformation-tree/input-type.md).

### Parameters

`baseOutputType` - The class type of [B](merge.md#B)

`compatibleOutputTypes` - A set of covariant classes of [B](merge.md#B)

**Return**
A tree which also covers all given [compatibleOutputTypes](merge.md#io.anima.transform$merge(io.anima.transform.TransformationTree((io.anima.transform.merge.A, io.anima.transform.merge.B)), java.lang.Class((io.anima.transform.merge.B)), kotlin.Array((java.lang.Class((io.anima.transform.merge.B)))))/compatibleOutputTypes)

`fun <A : `[`Immutable`](-immutable/index.md)`, reified B : `[`Immutable`](-immutable/index.md)`> `[`TransformationTree`](-transformation-tree/index.md)`<A, out B>.merge(vararg compatibleOutputTypes: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<out B>): `[`TransformationTree`](-transformation-tree/index.md)`<A, B>`

Creates a new tree which also covers covariant types to [B](merge.md#B).

The created tree keeps the [TransformationTree.inputType](-transformation-tree/input-type.md).
This is the inline reified version of [merge](./merge.md).

### Parameters

`compatibleOutputTypes` - A set of covariant classes of [B](merge.md#B)

**Return**
A tree which also covers all given [compatibleOutputTypes](merge.md#io.anima.transform$merge(io.anima.transform.TransformationTree((io.anima.transform.merge.A, io.anima.transform.merge.B)), kotlin.Array((java.lang.Class((io.anima.transform.merge.B)))))/compatibleOutputTypes)

