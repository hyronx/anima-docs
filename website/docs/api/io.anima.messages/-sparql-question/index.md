[anima](../../index.md) / [io.anima.messages](../index.md) / [SparqlQuestion](./index.md)

# SparqlQuestion

`class SparqlQuestion : `[`QuestionMessage`](../-question-message/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `SparqlQuestion(query: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, args: JsonObject? = null, questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`? = null, hash: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`? = null)` |

### Properties

| Name | Summary |
|---|---|
| [args](args.md) | `val args: JsonObject?` |
| [hash](hash.md) | `val hash: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) |
| [query](query.md) | `val query: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [questionId](question-id.md) | `val questionId: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [type](type.md) | `val type: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns the representation of a JSON serializable object in JSON.`fun toJsonObject(): JsonObject` |

### Companion Object Properties

| Name | Summary |
|---|---|
| [TYPE](-t-y-p-e.md) | `const val TYPE: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
