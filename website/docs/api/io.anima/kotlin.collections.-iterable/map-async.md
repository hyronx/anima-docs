[anima](../../index.md) / [io.anima](../index.md) / [kotlin.collections.Iterable](index.md) / [mapAsync](./map-async.md)

# mapAsync

`inline fun <T, S> `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<T>.mapAsync(crossinline handler: (element: T) -> S): `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<Future<S>>`
`inline fun <T, S> `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<T>.mapAsync(crossinline handler: (element: T, promise: Promise<S>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<Future<S>>`