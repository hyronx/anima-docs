[anima](../../index.md) / [io.anima.messages](../index.md) / [CacheResponse](./index.md)

# CacheResponse

`sealed class CacheResponse : `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

### Types

| Name | Summary |
|---|---|
| [Failure](-failure/index.md) | `class Failure : `[`CacheResponse`](./index.md) |
| [Ok](-ok/index.md) | `class Ok : `[`CacheResponse`](./index.md) |
| [Success](-success/index.md) | `class Success<T> : `[`CacheResponse`](./index.md) |

### Properties

| Name | Summary |
|---|---|
| [requestId](request-id.md) | `val requestId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [status](status.md) | `val status: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`open fun toJsonObject(): JsonObject` |
