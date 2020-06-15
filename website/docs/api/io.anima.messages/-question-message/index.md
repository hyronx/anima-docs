[anima](../../index.md) / [io.anima.messages](../index.md) / [QuestionMessage](./index.md)

# QuestionMessage

`interface QuestionMessage : `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

### Properties

| Name | Summary |
|---|---|
| [hash](hash.md) | `abstract val hash: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) |
| [questionId](question-id.md) | `abstract val questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [type](type.md) | `abstract val type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`open fun toJsonObject(): JsonObject` |

### Companion Object Properties

| Name | Summary |
|---|---|
| [hashDecoder](hash-decoder.md) | `val hashDecoder: `[`Decoder`](https://docs.oracle.com/javase/6/docs/api/java/util/Base64/Decoder.html) |
| [hashEncoder](hash-encoder.md) | `val hashEncoder: `[`Encoder`](https://docs.oracle.com/javase/6/docs/api/java/util/Base64/Encoder.html) |

### Inheritors

| Name | Summary |
|---|---|
| [GremlinQuestion](../-gremlin-question/index.md) | `class GremlinQuestion : `[`QuestionMessage`](./index.md) |
| [SparqlQuestion](../-sparql-question/index.md) | `class SparqlQuestion : `[`QuestionMessage`](./index.md) |
