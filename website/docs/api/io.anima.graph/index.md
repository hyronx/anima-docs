[anima](../index.md) / [io.anima.graph](./index.md)

## Package io.anima.graph

### Types

| Name | Summary |
|---|---|
| [AsyncRule](-async-rule/index.md) | Represents a validation and customization rule for a [Graph](-graph/index.md).`interface ~~AsyncRule~~` |
| [Edge](-edge/index.md) | `interface Edge<T, V> where T : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<T>, T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, V : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<V>, V : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html) |
| [EdgeToInVertexPairs](-edge-to-in-vertex-pairs.md) | `typealias EdgeToInVertexPairs = `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Pair`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-pair/index.html)`<`[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`>>` |
| [Graph](-graph/index.md) | `class Graph : `[`GraphMap`](-graph-map.md)`, `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [GraphMap](-graph-map.md) | `typealias GraphMap = `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, `[`EdgeToInVertexPairs`](-edge-to-in-vertex-pairs.md)`>` |
| [Layer](-layer/index.md) | `enum class Layer` |
| [MutableClassMap](-mutable-class-map.md) | `typealias MutableClassMap<T> = `[`MutableMap`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-map/index.html)`<`[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<*>, `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<T>>` |
| [MutableGraphMap](-mutable-graph-map.md) | `typealias MutableGraphMap = `[`MutableMap`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-map/index.html)`<`[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, `[`EdgeToInVertexPairs`](-edge-to-in-vertex-pairs.md)`>` |
| [Rule](-rule/index.md) | Represents a validation and customization rule for a [Graph](-graph/index.md).`interface Rule : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [Triple](-triple/index.md) | `data class Triple<LV : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, E : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, RV : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`>` |
| [Vertex](-vertex/index.md) | `interface Vertex<T> where T : `[`Comparable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-comparable/index.html)`<T>, T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html) |

### Extensions for External Classes

| Name | Summary |
|---|---|
| [kotlin.collections.Iterable](kotlin.collections.-iterable/index.md) |  |

### Functions

| Name | Summary |
|---|---|
| [collectOutVertices](collect-out-vertices.md) | `fun <T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`> `[`Graph`](-graph/index.md)`.collectOutVertices(vertex: T): `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>?` |
| [correct](correct.md) | Corrects this graph based on its rules in [Graph.rules](-graph/rules.md).`fun `[`Graph`](-graph/index.md)`.correct(): `[`Graph`](-graph/index.md) |
| [mergeAll](merge-all.md) | `fun `[`Graph`](-graph/index.md)`.mergeAll(others: `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<`[`Graph`](-graph/index.md)`>): `[`Graph`](-graph/index.md) |
