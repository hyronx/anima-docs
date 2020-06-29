[anima](../../index.md) / [io.anima.config](../index.md) / [WebFrontendConfig](./index.md)

# WebFrontendConfig

`data class WebFrontendConfig : `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `WebFrontendConfig(path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`? = null, allowRootFsAccess: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = false)` |

### Properties

| Name | Summary |
|---|---|
| [allowRootFsAccess](allow-root-fs-access.md) | `val allowRootFsAccess: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [path](path.md) | `val path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`?` |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`fun toJsonObject(): JsonObject` |
