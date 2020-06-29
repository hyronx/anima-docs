[anima](../index.md) / [io.anima.messages](./index.md)

## Package io.anima.messages

### Types

| Name | Summary |
|---|---|
| [AnswerMessage](-answer-message/index.md) | `interface AnswerMessage : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [AnswersCapsule](-answers-capsule/index.md) | `data class AnswersCapsule : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [CacheRequest](-cache-request/index.md) | `sealed class CacheRequest : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [CacheResponse](-cache-response/index.md) | `sealed class CacheResponse : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [CypherQuestion](-cypher-question/index.md) | `class CypherQuestion : `[`QuestionMessage`](-question-message/index.md) |
| [CypherQuestionCapsule](-cypher-question-capsule/index.md) | `data class CypherQuestionCapsule : `[`QuestionCapsule`](-question-capsule/index.md) |
| [FinalAnswer](-final-answer/index.md) | `data class FinalAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [GraphAnswer](-graph-answer/index.md) | `data class GraphAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [GremlinAnswer](-gremlin-answer/index.md) | `data class GremlinAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [GremlinQuestion](-gremlin-question/index.md) | `class GremlinQuestion : `[`QuestionMessage`](-question-message/index.md) |
| [HiveSendMessage](-hive-send-message/index.md) | `data class HiveSendMessage : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [ListAnswer](-list-answer/index.md) | `data class ListAnswer<T> : `[`AnswerMessage`](-answer-message/index.md) |
| [MapAnswer](-map-answer/index.md) | `data class MapAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [NoAnswer](-no-answer/index.md) | `data class NoAnswer : `[`AnswerMessage`](-answer-message/index.md) |
| [QuestionCapsule](-question-capsule/index.md) | `abstract class QuestionCapsule : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [QuestionMessage](-question-message/index.md) | `interface QuestionMessage : `[`JsonObjectSerializable`](../io.anima/-json-object-serializable/index.md) |
| [QuestionMessageCapsule](-question-message-capsule/index.md) | `data class QuestionMessageCapsule : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [SequenceAnswersCapsule](-sequence-answers-capsule/index.md) | `data class SequenceAnswersCapsule : `[`SequenceCapsule`](../io.anima.transform/-sequence-capsule/index.md)`<`[`AnswersCapsule`](-answers-capsule/index.md)`>` |
| [SetAnswer](-set-answer/index.md) | `data class SetAnswer<T> : `[`AnswerMessage`](-answer-message/index.md) |
| [SparqlQuestion](-sparql-question/index.md) | `class SparqlQuestion : `[`QuestionMessage`](-question-message/index.md) |
| [SparqlQuestionCapsule](-sparql-question-capsule/index.md) | `data class SparqlQuestionCapsule : `[`QuestionCapsule`](-question-capsule/index.md) |

### Extensions for External Classes

| Name | Summary |
|---|---|
| [io.vertx.core.json.JsonObject](io.vertx.core.json.-json-object/index.md) |  |

### Functions

| Name | Summary |
|---|---|
| [hiveRegisterMessage](hive-register-message.md) | `fun hiveRegisterMessage(address: `[`Address`](../io.anima/-address/index.md)`): `[`HiveSendMessage`](-hive-send-message/index.md) |
| [hiveUnregisterMessage](hive-unregister-message.md) | `fun hiveUnregisterMessage(address: `[`Address`](../io.anima/-address/index.md)`): `[`HiveSendMessage`](-hive-send-message/index.md) |
