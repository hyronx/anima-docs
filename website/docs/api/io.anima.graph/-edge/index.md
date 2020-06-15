[anima](../../index.md) / [io.anima.graph](../index.md) / [Edge](./index.md)

# Edge

`interface Edge<T, V> where T : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<T>, T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, V : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<V>, V : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)

### Properties

| Name | Summary |
|---|---|
| [data](data.md) | `abstract val data: T` |
| [metaEdges](meta-edges.md) | `abstract val metaEdges: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Edge`](./index.md)`<*, *>>` |
| [outVertex](out-vertex.md) | `abstract val outVertex: `[`Vertex`](../-vertex/index.md)`<V>` |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun <T, V> create(data: T, outVertex: `[`Vertex`](../-vertex/index.md)`<V>, metaEdges: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Edge`](./index.md)`<*, *>>): `[`Edge`](./index.md)`<T, V> where T : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<T>, T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, V : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<V>, V : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)<br>`fun <T, V> create(data: T, outVertex: `[`Vertex`](../-vertex/index.md)`<V>, vararg metaEdges: `[`Edge`](./index.md)`<*, *>): `[`Edge`](./index.md)`<T, V> where T : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<T>, T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, V : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<V>, V : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html) |
