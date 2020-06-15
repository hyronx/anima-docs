[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationTreeBuilder](./index.md)

# TransformationTreeBuilder

`class TransformationTreeBuilder`

### Properties

| Name | Summary |
|---|---|
| [treeCache](tree-cache.md) | `var treeCache: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`TransformationType`](../-transformation-type.md)`<*, *>, `[`TransformationTree`](../-transformation-tree/index.md)`<*, *>>` |

### Functions

| Name | Summary |
|---|---|
| [build](build.md) | Builds the [TransformationTree](../-transformation-tree/index.md).`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> build(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, customBuilder: (`[`TransformationTreeBuilder`](./index.md)`.(`[`TransformationTree`](../-transformation-tree/index.md)`<A, B>) -> `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>)? = null): `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>`<br>`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> build(customBuilder: (`[`TransformationTreeBuilder`](./index.md)`.(`[`TransformationTree`](../-transformation-tree/index.md)`<A, B>) -> `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>)? = null): `[`TransformationTree`](../-transformation-tree/index.md)`<A, B>` |
| [findPaths](find-paths.md) | `fun <B : `[`Immutable`](../-immutable/index.md)`, C : `[`Immutable`](../-immutable/index.md)`, D : `[`Immutable`](../-immutable/index.md)`> `[`TransformationTreeNode`](../-transformation-tree-node/index.md)`<C, D>.findPaths(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<D>, targetOutputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`TransformationTreeNode`](../-transformation-tree-node/index.md)`<D, *>>?` |
| [isNotCyclic](is-not-cyclic.md) | `fun <C : `[`Immutable`](../-immutable/index.md)`, D : `[`Immutable`](../-immutable/index.md)`, E : `[`Immutable`](../-immutable/index.md)`> isNotCyclic(parent: `[`TransformationTreeNode`](../-transformation-tree-node/index.md)`<C, D>, currentOutputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<E>): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [removeSelfFromTree](remove-self-from-tree.md) | `fun <C : `[`Immutable`](../-immutable/index.md)`, D : `[`Immutable`](../-immutable/index.md)`> `[`TransformationTreeNode`](../-transformation-tree-node/index.md)`<C, D>.removeSelfFromTree(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun create(currentTransformations: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`TransformationType`](../-transformation-type.md)`<*, *>, `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Transformation`](../-transformation/index.md)`<*, *>>>? = null): `[`TransformationTreeBuilder`](./index.md) |
