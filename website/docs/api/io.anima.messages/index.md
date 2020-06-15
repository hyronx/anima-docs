[anima](../index.md) / [io.anima.messages](./index.md)

## Package io.anima.messages

### Types

| Name | Summary |
|---|---|
| [AnswerMessage](-answer-message/index.md) | `interface AnswerMessage : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [CacheRequest](-cache-request/index.md) | `sealed class CacheRequest : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [CacheResponse](-cache-response/index.md) | `sealed class CacheResponse : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [GraphAnswer](-graph-answer/index.md) | `data class GraphAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [GremlinAnswer](-gremlin-answer/index.md) | `data class GremlinAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [GremlinQuestion](-gremlin-question/index.md) | `class GremlinQuestion : `[`QuestionMessage`](-question-message/index.md) |
| [ListAnswer](-list-answer/index.md) | `data class ListAnswer<T> : `[`AnswerMessage`](-answer-message/index.md) |
| [MapAnswer](-map-answer/index.md) | `data class MapAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [NoAnswer](-no-answer/index.md) | `data class NoAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [QuestionMessage](-question-message/index.md) | `interface QuestionMessage : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [SetAnswer](-set-answer/index.md) | `data class SetAnswer<T> : `[`AnswerMessage`](-answer-message/index.md) |
| [SparqlQuestion](-sparql-question/index.md) | `class SparqlQuestion : `[`QuestionMessage`](-question-message/index.md) |

### Extensions for External Classes

| Name | Summary |
|---|---|
| [io.vertx.core.json.JsonObject](io.vertx.core.json.-json-object/index.md) |  |
