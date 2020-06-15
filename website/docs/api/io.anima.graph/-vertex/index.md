[anima](../../index.md) / [io.anima.graph](../index.md) / [Vertex](./index.md)

# Vertex

`interface Vertex<T> where T : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<T>, T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)

### Properties

| Name | Summary |
|---|---|
| [data](data.md) | `abstract val data: T` |
| [outEdges](out-edges.md) | `abstract val outEdges: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Edge`](../-edge/index.md)`<*, *>>` |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun <T> create(data: T, outEdges: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Edge`](../-edge/index.md)`<*, *>>): `[`Vertex`](./index.md)`<T> where T : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<T>, T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)<br>`fun <T> create(data: T, vararg outEdges: `[`Edge`](../-edge/index.md)`<*, *>): `[`Vertex`](./index.md)`<T> where T : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<T>, T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html) |
