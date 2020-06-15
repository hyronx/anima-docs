[anima](../../index.md) / [io.anima](../index.md) / [AnimaVerticle](index.md) / [start](./start.md)

# start

`protected abstract fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Configures and sets up this verticle.

Override this verticle to set up [io.vertx.core.eventbus.MessageConsumer](#)s or do any
other setup required for this verticle. If your verticle only runs once then let
its magic happen in this method.

### Parameters

`startPromise` - A promise returning the completion or failure of the [start](./start.md) method

`currentConfig` - The current configuration as processed by [processConfig](process-config.md)`open fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Starts a Vert.x verticle.

**See Also**

[AbstractVerticle.start](#)

