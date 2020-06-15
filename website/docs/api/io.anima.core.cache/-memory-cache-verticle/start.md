[anima](../../index.md) / [io.anima.core.cache](../index.md) / [MemoryCacheVerticle](index.md) / [start](./start.md)

# start

`protected fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Configures and sets up this verticle.

Override this verticle to set up [io.vertx.core.eventbus.MessageConsumer](#)s or do any
other setup required for this verticle. If your verticle only runs once then let
its magic happen in this method.

### Parameters

`startPromise` - A promise returning the completion or failure of the [start](../../io.anima/-anima-verticle/start.md) method

`currentConfig` - The current configuration as processed by [processConfig](../../io.anima/-anima-verticle/process-config.md)