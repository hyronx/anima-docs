[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationTreeRoot](./index.md)

# TransformationTreeRoot

`class TransformationTreeRoot<A : `[`Immutable`](../-immutable/index.md)`> : `[`TransformationTreeNode`](../-transformation-tree-node/index.md)`<A, A>`

The root of a tree of functions

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | The root of a tree of functions`TransformationTreeRoot(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, statusAddress: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, context: `[`TransformationContext`](../-transformation-context/index.md)` = TransformationContext(statusAddress, listOf()), transformations: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Transformation`](../-transformation/index.md)`<A, A>> = setOf())` |

### Properties

| Name | Summary |
|---|---|
| [context](context.md) | `val context: `[`TransformationContext`](../-transformation-context/index.md) |
| [type](type.md) | `val type: `[`TransformationType`](../-transformation-type.md)`<A, A>` |

### Functions

| Name | Summary |
|---|---|
| [handler](handler.md) | Calls its transform elements and the next element in the chain`fun handler(input: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<*>>` |
