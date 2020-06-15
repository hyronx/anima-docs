[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](index.md) / [publishStatus](./publish-status.md)

# publishStatus

`open fun publishStatus(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, additionalInfo: JsonObject = jsonObjectOf(), deliveryOptions: DeliveryOptions = deliveryOptionsOf()): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Sends a status message.

### Parameters

`message` - The message to send

`additionalInfo` - Additional attributes about this status

`deliveryOptions` - Custom delivery options for the Vert.x Event Bus