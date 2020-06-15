[anima](../../index.md) / [io.anima](../index.md) / [AnimaVerticle](index.md) / [afterStart](./after-start.md)

# afterStart

`protected open fun afterStart(firstConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Gets called after [start](start.md) has finished.

Override this method to do some cleanup for the initialization process.
This isn't necessary in most cases.
The configuration isn't updated for this method.
To do the final cleanup before verticle shutdown override a [stop](stop.md) variant.

### Parameters

`firstConfig` - The first configuration after application startup