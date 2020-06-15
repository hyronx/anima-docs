[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationContext](./index.md)

# TransformationContext

`data class TransformationContext : `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>`

Immutable contextual information for a transformation

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Immutable contextual information for a transformation`TransformationContext(statusAddress: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, previousTypes: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`TransformationType`](../-transformation-type.md)`<*, *>>, contextData: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`> = mapOf())` |

### Properties

| Name | Summary |
|---|---|
| [contextData](context-data.md) | `val contextData: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>` |
| [previousTypes](previous-types.md) | `val previousTypes: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`TransformationType`](../-transformation-type.md)`<*, *>>` |
| [statusAddress](status-address.md) | `val statusAddress: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [plus](../plus.md) | Appends a [TransformationType](../-transformation-type.md) of a previously processed transformation type.`operator fun `[`TransformationContext`](./index.md)`.plus(previousType: `[`TransformationType`](../-transformation-type.md)`<*, *>): `[`TransformationContext`](./index.md) |
