[anima](../../index.md) / [io.anima.core.mind.gremlin](../index.md) / [AnimaTinkerElement](./index.md)

# AnimaTinkerElement

`sealed class AnimaTinkerElement`

### Properties

| Name | Summary |
|---|---|
| [id](id.md) | `abstract val id: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [label](label.md) | `abstract val label: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [properties](properties.md) | `abstract val properties: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>` |

### Inheritors

| Name | Summary |
|---|---|
| [AnimaTinkerEdge](../-anima-tinker-edge/index.md) | `data class AnimaTinkerEdge : `[`AnimaTinkerElement`](./index.md) |
| [AnimaTinkerVertex](../-anima-tinker-vertex/index.md) | `data class AnimaTinkerVertex : `[`AnimaTinkerElement`](./index.md) |
