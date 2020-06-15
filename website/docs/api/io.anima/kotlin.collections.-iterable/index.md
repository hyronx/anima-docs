[anima](../../index.md) / [io.anima](../index.md) / [kotlin.collections.Iterable](./index.md)

### Extensions for kotlin.collections.Iterable

| Name | Summary |
|---|---|
| [mapAsync](map-async.md) | `fun <T, S> `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<T>.mapAsync(handler: (element: T) -> S): `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<Future<S>>`<br>`fun <T, S> `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<T>.mapAsync(handler: (element: T, promise: Promise<S>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<Future<S>>` |
| [onAllComplete](on-all-complete.md) | `fun <T> `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<Future<T>>.onAllComplete(completionHandler: (result: AsyncResult<CompositeFuture>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [onAllCompleteAndIgnoreResult](on-all-complete-and-ignore-result.md) | `fun <T> `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<Future<T>>.onAllCompleteAndIgnoreResult(completionHandler: (result: AsyncResult<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [toCompositeFuture](to-composite-future.md) | `fun <T> `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<Future<T>>.toCompositeFuture(): CompositeFuture` |
| [toJsonArray](to-json-array.md) | `fun `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<*>.toJsonArray(customDeserializer: ((`[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`?) -> JsonObject)? = null): JsonArray` |