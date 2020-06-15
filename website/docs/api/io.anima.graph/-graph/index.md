[anima](../../index.md) / [io.anima.graph](../index.md) / [Graph](./index.md)

# Graph

`class Graph : `[`GraphMap`](../-graph-map.md)`, `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

### Types

| Name | Summary |
|---|---|
| [Builder](-builder/index.md) | `class Builder` |

### Properties

| Name | Summary |
|---|---|
| [isValid](is-valid.md) | `val isValid: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [metaGraph](meta-graph.md) | `val metaGraph: `[`GraphMap`](../-graph-map.md) |
| [rules](rules.md) | `var rules: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Rule`](../-rule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [clone](clone.md) | `fun clone(graph: `[`GraphMap`](../-graph-map.md)` = this.graph.toMap(), metaGraph: `[`GraphMap`](../-graph-map.md)` = this.metaGraph.toMap(), rules: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Rule`](../-rule/index.md)`> = this.rules.toSet(), isValid: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = this.isValid): `[`Graph`](./index.md) |
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`fun toJsonObject(): JsonObject` |
| [toString](to-string.md) | `fun toString(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun create(builder: Builder.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Graph`](./index.md) |

### Extension Functions

| Name | Summary |
|---|---|
| [collectOutVertices](../collect-out-vertices.md) | `fun <T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`> `[`Graph`](./index.md)`.collectOutVertices(vertex: T): `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>?` |
| [correct](../correct.md) | Corrects this graph based on its rules in [Graph.rules](rules.md).`fun `[`Graph`](./index.md)`.correct(): `[`Graph`](./index.md) |
| [mergeAll](../merge-all.md) | `fun `[`Graph`](./index.md)`.mergeAll(others: `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<`[`Graph`](./index.md)`>): `[`Graph`](./index.md) |
