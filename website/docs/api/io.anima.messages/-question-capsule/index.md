[anima](../../index.md) / [io.anima.messages](../index.md) / [QuestionCapsule](./index.md)

# QuestionCapsule

`abstract class QuestionCapsule : `[`Immutable`](../../io.anima.transform/-immutable/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `QuestionCapsule()` |

### Properties

| Name | Summary |
|---|---|
| [hash](hash.md) | `abstract val hash: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) |
| [questionId](question-id.md) | `abstract val questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [CypherQuestionCapsule](../-cypher-question-capsule/index.md) | `data class CypherQuestionCapsule : `[`QuestionCapsule`](./index.md) |
| [SparqlQuestionCapsule](../-sparql-question-capsule/index.md) | `data class SparqlQuestionCapsule : `[`QuestionCapsule`](./index.md) |
