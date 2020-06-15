[anima](../../index.md) / [io.anima](../index.md) / [AnimaVerticle](index.md) / [beforeStart](./before-start.md)

# beforeStart

`protected open fun beforeStart(firstConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Gets called before [start](start.md) is called.

Override this method to do some pre-initialising. This isn't necessary in most cases.
The configuration isn't updated for this method.

### Parameters

`firstConfig` - The first configuration after application startup