[anima](../../index.md) / [io.anima.messages](../index.md) / [NoAnswer](./index.md)

# NoAnswer

`data class NoAnswer : `[`AnswerMessage`](../-answer-message/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `NoAnswer(questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`)` |

### Properties

| Name | Summary |
|---|---|
| [isConcurrentResult](is-concurrent-result.md) | Must be true if this answer is one of multiple answer messages related to one question and these answers are sent concurrently.`val isConcurrentResult: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [isSequential](is-sequential.md) | Must be true if this answer is one of multiple answer messages related to one question and these answers are given sequential.`val isSequential: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [questionId](question-id.md) | The question ID to which this answer belongs`var questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [type](type.md) | The type of the answer`val type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [clone](clone.md) | Clones this answer message, optionally changing the [questionId](../-answer-message/clone.md#io.anima.messages.AnswerMessage$clone(kotlin.String)/questionId).`fun clone(questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`NoAnswer`](./index.md) |

### Companion Object Properties

| Name | Summary |
|---|---|
| [TYPE](-t-y-p-e.md) | `const val TYPE: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
