[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationTree](./index.md)

# TransformationTree

`data class TransformationTree<A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> : `[`Transformation`](../-transformation/index.md)`<A, B>`

A tree of functions

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | A tree of functions`TransformationTree(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>)` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | The input type for this tree`val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>` |
| [leaves](leaves.md) | Gathers all leaves of the tree.`val leaves: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`TransformationTreeChild`](../-transformation-tree-child/index.md)`<*, B>>` |
| [outputType](output-type.md) | The output type for this tree`val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>` |
| [rootNode](root-node.md) | The root node of the tree`var rootNode: `[`TransformationTreeRoot`](../-transformation-tree-root/index.md)`<A>` |
| [statusAddress](status-address.md) | The address where status message are sent to`val statusAddress: `[`TransformationStatusAddress`](../-transformation-status-address/index.md)`<A, B>` |

### Functions

| Name | Summary |
|---|---|
| [freeze](freeze.md) | Freezes this tree.`fun freeze(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [invoke](invoke.md) | Calls the transform tree`fun invoke(inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>, context: `[`TransformationContext`](../-transformation-context/index.md)`): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>!>` |
| [transform](transform.md) | This method does nothing. Use the [invoke](invoke.md) method instead.`fun transform(input: A, outputPromise: Promise<B>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | Creates a new [TransformationTree](./index.md).`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> create(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>): `[`TransformationTree`](./index.md)`<A, B>`<br>`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> create(vertx: Vertx): `[`TransformationTree`](./index.md)`<A, B>` |

### Extension Functions

| Name | Summary |
|---|---|
| [compose](../compose.md) | Creates a new transformation tree for [A](../compose.md#A) to [C](../compose.md#C) by reusing this tree.`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`, C : `[`Immutable`](../-immutable/index.md)`> `[`TransformationTree`](./index.md)`<A, B>.compose(nextOutputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<C>, outputMapper: (previousOutputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>, outputPromise: Promise<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)` = { i, o -> o.complete(i) }): `[`TransformationTree`](./index.md)`<A, C>` |
| [merge](../merge.md) | Creates a new tree which also covers covariant types to [B](../merge.md#B).`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`TransformationTree`](./index.md)`<A, out B>.merge(baseOutputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, vararg compatibleOutputTypes: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<out B>): `[`TransformationTree`](./index.md)`<A, B>`<br>`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`TransformationTree`](./index.md)`<A, out B>.merge(vararg compatibleOutputTypes: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<out B>): `[`TransformationTree`](./index.md)`<A, B>` |
| [walk](../walk.md) | `fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`TransformationTree`](./index.md)`<A, B>.~~walk~~(walker: (`[`TransformationTreeNode`](../-transformation-tree-node/index.md)`<*, *>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
