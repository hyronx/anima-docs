[anima](../../index.md) / [io.anima](../index.md) / [JsonObjectSerializable](./index.md)

# JsonObjectSerializable

`interface JsonObjectSerializable`

Represents a JSON serializable object

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`abstract fun toJsonObject(): JsonObject` |

### Inheritors

| Name | Summary |
|---|---|
| [AnswerMessage](../../io.anima.messages/-answer-message/index.md) | `interface AnswerMessage : `[`JsonObjectSerializable`](./index.md) |
| [CacheRequest](../../io.anima.messages/-cache-request/index.md) | `sealed class CacheRequest : `[`JsonObjectSerializable`](./index.md) |
| [CacheResponse](../../io.anima.messages/-cache-response/index.md) | `sealed class CacheResponse : `[`JsonObjectSerializable`](./index.md) |
| [DataConfig](../../io.anima.core.config/-data-config/index.md) | `data class DataConfig : `[`JsonObjectSerializable`](./index.md) |
| [DrawIoConfig](../../io.anima.config/-draw-io-config/index.md) | `data class DrawIoConfig : `[`JsonObjectSerializable`](./index.md) |
| [Graph](../../io.anima.graph/-graph/index.md) | `class Graph : `[`GraphMap`](../../io.anima.graph/-graph-map.md)`, `[`JsonObjectSerializable`](./index.md) |
| [GraphStoreConfig](../../io.anima.core.config/-graph-store-config/index.md) | `data class GraphStoreConfig : `[`JsonObjectSerializable`](./index.md) |
| [GremlinConfig](../../io.anima.core.config/-gremlin-config/index.md) | `data class GremlinConfig : `[`JsonObjectSerializable`](./index.md) |
| [HiveConnectionInfo](../../io.anima.core.config/-hive-connection-info/index.md) | `data class HiveConnectionInfo : `[`JsonObjectSerializable`](./index.md) |
| [Immutable](../../io.anima.transform/-immutable/index.md) | Represents an immutable, serializable and cloneable type.`interface Immutable : `[`Cloneable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-cloneable/index.html)`, `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, `[`JsonObjectSerializable`](./index.md) |
| [InstanceConfig](../../io.anima.core.config/-instance-config/index.md) | `data class InstanceConfig : `[`JsonObjectSerializable`](./index.md) |
| [MindConfig](../../io.anima.core.config/-mind-config/index.md) | `data class MindConfig : `[`JsonObjectSerializable`](./index.md) |
| [ModuleConfig](../../io.anima.core.config/-module-config/index.md) | `data class ModuleConfig : `[`JsonObjectSerializable`](./index.md) |
| [QuestionMessage](../../io.anima.messages/-question-message/index.md) | `interface QuestionMessage : `[`JsonObjectSerializable`](./index.md) |
| [RedisConfig](../../io.anima.config/-redis-config/index.md) | `data class RedisConfig : `[`JsonObjectSerializable`](./index.md) |
| [Rule](../../io.anima.graph/-rule/index.md) | Represents a validation and customization rule for a [Graph](../../io.anima.graph/-graph/index.md).`interface Rule : `[`JsonObjectSerializable`](./index.md) |
| [RulesConfig](../../io.anima.config/-rules-config/index.md) | `data class RulesConfig : `[`JsonObjectSerializable`](./index.md) |
| [WebApiConfig](../../io.anima.core.config/-web-api-config/index.md) | `data class WebApiConfig : `[`JsonObjectSerializable`](./index.md) |
| [WebConfig](../../io.anima.core.config/-web-config/index.md) | `data class WebConfig : `[`JsonObjectSerializable`](./index.md) |
