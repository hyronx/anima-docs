[anima](../../index.md) / [io.anima.core.config](../index.md) / [MindConfig](./index.md)

# MindConfig

`data class MindConfig : `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `MindConfig(data: `[`DataConfig`](../-data-config/index.md)` = DataConfig(), web: `[`WebConfig`](../-web-config/index.md)` = WebConfig(), gremlin: `[`GremlinConfig`](../-gremlin-config/index.md)` = GremlinConfig())` |

### Properties

| Name | Summary |
|---|---|
| [data](data.md) | `val data: `[`DataConfig`](../-data-config/index.md) |
| [gremlin](gremlin.md) | `val gremlin: `[`GremlinConfig`](../-gremlin-config/index.md) |
| [web](web.md) | `val web: `[`WebConfig`](../-web-config/index.md) |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`fun toJsonObject(): JsonObject` |
