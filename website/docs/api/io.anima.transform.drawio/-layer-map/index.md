[anima](../../index.md) / [io.anima.transform.drawio](../index.md) / [LayerMap](./index.md)

# LayerMap

`data class LayerMap`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `LayerMap(meta: `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`Cell`](../-cell/index.md)`> = mutableListOf(), abstract: `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`Cell`](../-cell/index.md)`> = mutableListOf(), real: `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`Cell`](../-cell/index.md)`> = mutableListOf())` |

### Properties

| Name | Summary |
|---|---|
| [abstract](abstract.md) | `val abstract: `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`Cell`](../-cell/index.md)`>` |
| [meta](meta.md) | `val meta: `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`Cell`](../-cell/index.md)`>` |
| [real](real.md) | `val real: `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`Cell`](../-cell/index.md)`>` |

### Extension Functions

| Name | Summary |
|---|---|
| [get](../get.md) | `operator fun `[`LayerMap`](./index.md)`.get(layer: `[`Layer`](../../io.anima.graph/-layer/index.md)`): `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`Cell`](../-cell/index.md)`>` |
| [removeIf](../remove-if.md) | `fun `[`LayerMap`](./index.md)`.removeIf(finder: (`[`Cell`](../-cell/index.md)`) -> `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [toDrawIoGraph](../to-draw-io-graph.md) | `fun `[`LayerMap`](./index.md)`.toDrawIoGraph(): `[`Graph`](../-graph/index.md) |
