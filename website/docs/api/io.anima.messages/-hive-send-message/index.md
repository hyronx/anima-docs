[anima](../../index.md) / [io.anima.messages](../index.md) / [HiveSendMessage](./index.md)

# HiveSendMessage

`data class HiveSendMessage : `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `HiveSendMessage(address: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, body: `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)`, type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "publish")`<br>`HiveSendMessage(address: `[`Address`](../../io.anima/-address/index.md)`, body: JsonObject, type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "publish")`<br>`HiveSendMessage(address: `[`Address`](../../io.anima/-address/index.md)`, body: `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)`, type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "publish")`<br>`HiveSendMessage(address: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, body: JsonObject, type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "publish")` |

### Properties

| Name | Summary |
|---|---|
| [address](address.md) | `val address: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [body](body.md) | `val body: JsonObject` |
| [type](type.md) | `val type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`fun toJsonObject(): JsonObject` |
