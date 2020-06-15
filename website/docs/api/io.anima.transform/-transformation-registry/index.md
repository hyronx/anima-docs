[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationRegistry](./index.md)

# TransformationRegistry

`object TransformationRegistry`

### Properties

| Name | Summary |
|---|---|
| [registeredTransformations](registered-transformations.md) | `val registeredTransformations: `[`ConcurrentHashMap`](https://docs.oracle.com/javase/6/docs/api/java/util/concurrent/ConcurrentHashMap.html)`<`[`TransformationType`](../-transformation-type.md)`<*, *>, `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Transformation`](../-transformation/index.md)`<*, *>>>` |

### Functions

| Name | Summary |
|---|---|
| [register](register.md) | `fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`Transformation`](../-transformation/index.md)`<A, B>.register(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [unregister](unregister.md) | `fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> `[`Transformation`](../-transformation/index.md)`<A, B>.unregister(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
