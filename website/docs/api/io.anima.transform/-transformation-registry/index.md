[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationRegistry](./index.md)

# TransformationRegistry

`object TransformationRegistry`

### Properties

| Name | Summary |
|---|---|
| [transformationsView](transformations-view.md) | `val transformationsView: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`TransformationType`](../-transformation-type.md)`<*, *>, `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Transformation`](../-transformation/index.md)`<*, *>>>` |

### Functions

| Name | Summary |
|---|---|
| [get](get.md) | `operator fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> get(type: `[`TransformationType`](../-transformation-type.md)`<A, B>): `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Transformation`](../-transformation/index.md)`<A, B>>?` |
| [register](register.md) | `fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`Transformation`](../-transformation/index.md)`<A, B>.register(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [unregister](unregister.md) | `fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`Transformation`](../-transformation/index.md)`<A, B>.unregister(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
