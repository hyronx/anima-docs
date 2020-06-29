[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationTreeNode](./index.md)

# TransformationTreeNode

`abstract class TransformationTreeNode<C : `[`Immutable`](../-immutable/index.md)`, D : `[`Immutable`](../-immutable/index.md)`>`

A single element in the functions chain.

You doesn't usually instantiate this class directly. It is created by [].

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | A single element in the functions chain.`TransformationTreeNode()` |

### Properties

| Name | Summary |
|---|---|
| [cachedResults](cached-results.md) | <ul><li>A map of flattened results for some input from previous computations</li></ul>`var cachedResults: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<C>, `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<D>>` |
| [children](children.md) | Pointers to the children of this element`var children: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`TransformationTreeNode`](./index.md)`<D, *>>` |
| [context](context.md) | `abstract val context: `[`TransformationContext`](../-transformation-context/index.md) |
| [hasChildren](has-children.md) | `val hasChildren: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [isFrozen](is-frozen.md) | `var isFrozen: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [isLeaf](is-leaf.md) | `val isLeaf: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [parent](parent.md) | `var parent: `[`TransformationTreeNode`](./index.md)`<*, C>?` |
| [siblings](siblings.md) | `val siblings: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`TransformationTreeNode`](./index.md)`<C, *>>` |
| [type](type.md) | `abstract val type: `[`TransformationType`](../-transformation-type.md)`<C, D>` |

### Functions

| Name | Summary |
|---|---|
| [callChildren](call-children.md) | `fun callChildren(input: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<D>, promise: Promise<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<*>>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [freeze](freeze.md) | Recursively freezes the whole tree`open fun freeze(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [handler](handler.md) | Calls its transform elements and the next element in the chain`abstract fun handler(input: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<C>): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<*>>` |

### Inheritors

| Name | Summary |
|---|---|
| [TransformationTreeChild](../-transformation-tree-child/index.md) | `data class TransformationTreeChild<C : `[`Immutable`](../-immutable/index.md)`, D : `[`Immutable`](../-immutable/index.md)`> : `[`TransformationTreeNode`](./index.md)`<C, D>` |
| [TransformationTreeRoot](../-transformation-tree-root/index.md) | The root of a tree of functions`class TransformationTreeRoot<A : `[`Immutable`](../-immutable/index.md)`> : `[`TransformationTreeNode`](./index.md)`<A, A>` |
