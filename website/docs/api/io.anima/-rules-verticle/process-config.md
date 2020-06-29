[anima](../../index.md) / [io.anima](../index.md) / [RulesVerticle](index.md) / [processConfig](./process-config.md)

# processConfig

`fun processConfig(fullConfig: JsonObject): JsonObject`

Processes and customizes the full top level configuration object for the [start](../-anima-verticle/start.md) method.

Override this method to customize the configuration you need. Another option is to simply
return [fullConfig](../-anima-verticle/process-config.md#io.anima.AnimaVerticle$processConfig(io.vertx.core.json.JsonObject)/fullConfig) which gives you access to the full config in [start](../-anima-verticle/start.md). This isn't meant
to be used as some security feature as it isn't secure in anyway. Any module gets full access
to the configuration so *DON'T* store any sensitive transform in there.

### Parameters

`fullConfig` - The full top level configuration as a [JsonObject](#)

**Return**
A customized configuration

