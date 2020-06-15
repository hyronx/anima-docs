[anima](../../../index.md) / [io.anima.messages](../../index.md) / [CacheRequest](../index.md) / [Save](./index.md)

# Save

`class Save<T> : `[`CacheRequest`](../index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `Save(key: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, value: T, id: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = UUID.randomUUID().toString())` |

### Properties

| Name | Summary |
|---|---|
| [value](value.md) | `val value: T` |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`fun toJsonObject(): JsonObject` |
