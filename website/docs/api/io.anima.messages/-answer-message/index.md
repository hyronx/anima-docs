[anima](../../index.md) / [io.anima.messages](../index.md) / [AnswerMessage](./index.md)

# AnswerMessage

`interface AnswerMessage : `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

### Properties

| Name | Summary |
|---|---|
| [isConcurrentResult](is-concurrent-result.md) | Must be true if this answer is one of multiple answer messages related to one question and these answers are sent concurrently.`open val isConcurrentResult: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [isSequential](is-sequential.md) | Must be true if this answer is one of multiple answer messages related to one question and these answers are given sequential.`abstract val isSequential: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [isSingleResult](is-single-result.md) | Must be true if this answer is the only answer message related to one question.`open val isSingleResult: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [questionId](question-id.md) | The question ID to which this answer belongs`abstract val questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [sequentialId](sequential-id.md) | This ID represents the index of this answer message in a sequential answer and should only be set if [isSequential](is-sequential.md) is true.`open val sequentialId: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`?` |
| [type](type.md) | The type of the answer`abstract val type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [clone](clone.md) | Clones this answer message, optionally changing the [questionId](clone.md#io.anima.messages.AnswerMessage$clone(kotlin.String)/questionId).`abstract fun clone(questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = this.questionId): `[`AnswerMessage`](./index.md) |
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`open fun toJsonObject(): JsonObject` |

### Inheritors

| Name | Summary |
|---|---|
| [GraphAnswer](../-graph-answer/index.md) | `data class GraphAnswer : `[`AnswerMessage`](./index.md) |
| [GremlinAnswer](../-gremlin-answer/index.md) | `data class GremlinAnswer : `[`AnswerMessage`](./index.md) |
| [ListAnswer](../-list-answer/index.md) | `data class ListAnswer<T> : `[`AnswerMessage`](./index.md) |
| [MapAnswer](../-map-answer/index.md) | `data class MapAnswer : `[`AnswerMessage`](./index.md) |
| [NoAnswer](../-no-answer/index.md) | `data class NoAnswer : `[`AnswerMessage`](./index.md) |
| [SetAnswer](../-set-answer/index.md) | `data class SetAnswer<T> : `[`AnswerMessage`](./index.md) |
