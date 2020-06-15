[anima](../../index.md) / [io.anima.messages](../index.md) / [MapAnswer](./index.md)

# MapAnswer

`data class MapAnswer : `[`AnswerMessage`](../-answer-message/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `MapAnswer(questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, result: JsonObject, isSequential: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = false, sequentialId: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`? = null, isConcurrentResult: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = true, isSingleResult: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = false)` |

### Properties

| Name | Summary |
|---|---|
| [isConcurrentResult](is-concurrent-result.md) | Must be true if this answer is one of multiple answer messages related to one question and these answers are sent concurrently.`val isConcurrentResult: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [isSequential](is-sequential.md) | Must be true if this answer is one of multiple answer messages related to one question and these answers are given sequential.`val isSequential: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [isSingleResult](is-single-result.md) | Must be true if this answer is the only answer message related to one question.`val isSingleResult: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [questionId](question-id.md) | The question ID to which this answer belongs`var questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [result](result.md) | `val result: JsonObject` |
| [sequentialId](sequential-id.md) | This ID represents the index of this answer message in a sequential answer and should only be set if [isSequential](../-answer-message/is-sequential.md) is true.`val sequentialId: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`?` |
| [type](type.md) | The type of the answer`val type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [clone](clone.md) | Clones this answer message, optionally changing the [questionId](../-answer-message/clone.md#io.anima.messages.AnswerMessage$clone(kotlin.String)/questionId).`fun clone(questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`MapAnswer`](./index.md) |
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`fun toJsonObject(): JsonObject` |

### Companion Object Properties

| Name | Summary |
|---|---|
| [TYPE](-t-y-p-e.md) | `const val TYPE: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
