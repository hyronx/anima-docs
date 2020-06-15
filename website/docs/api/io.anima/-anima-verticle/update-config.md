[anima](../../index.md) / [io.anima](../index.md) / [AnimaVerticle](index.md) / [updateConfig](./update-config.md)

# updateConfig

`protected fun JsonObject.updateConfig(newFullConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Updates the configuration with the new one.

You must pass the top level configuration as it will be merged
with current top level configuration. The updating happens
through the event bus at address [Address.ConfigUpdate](../-address/-config-update.md).

### Parameters

`newFullConfig` - The new top level configuration