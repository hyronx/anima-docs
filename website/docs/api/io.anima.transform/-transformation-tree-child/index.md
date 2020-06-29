[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationTreeChild](./index.md)

# TransformationTreeChild

`data class TransformationTreeChild<C : `[`Immutable`](../-immutable/index.md)`, D : `[`Immutable`](../-immutable/index.md)`> : `[`TransformationTreeNode`](../-transformation-tree-node/index.md)`<C, D>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `TransformationTreeChild(type: `[`TransformationType`](../-transformation-type.md)`<C, D>, transformations: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Transformation`](../-transformation/index.md)`<C, D>>, context: `[`TransformationContext`](../-transformation-context/index.md)`)` |

### Properties

| Name | Summary |
|---|---|
| [context](context.md) | `val context: `[`TransformationContext`](../-transformation-context/index.md) |
| [transformations](transformations.md) | The set of transform objects corresponding to this element`val transformations: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Transformation`](../-transformation/index.md)`<C, D>>` |
| [type](type.md) | The input to output type definition`val type: `[`TransformationType`](../-transformation-type.md)`<C, D>` |

### Functions

| Name | Summary |
|---|---|
| [freeze](freeze.md) | Recursively freezes the whole tree`fun freeze(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [handler](handler.md) | Calls its transform elements and the next element in the chain`fun handler(input: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<C>): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<*>>` |
