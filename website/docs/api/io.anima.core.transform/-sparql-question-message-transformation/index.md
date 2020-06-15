[anima](../../index.md) / [io.anima.core.transform](../index.md) / [SparqlQuestionMessageTransformation](./index.md)

# SparqlQuestionMessageTransformation

`class SparqlQuestionMessageTransformation : `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`QuestionMessageCapsule`](../-question-message-capsule/index.md)`, `[`SparqlQuestionCapsule`](../-sparql-question-capsule/index.md)`>`

Transforms question messages to SPARQL questions for the transformation system if possible.

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Transforms question messages to SPARQL questions for the transformation system if possible.`SparqlQuestionMessageTransformation()` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | The input type for this transformation`val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`QuestionMessageCapsule`](../-question-message-capsule/index.md)`>` |
| [outputType](output-type.md) | The output type for this transformation`val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`SparqlQuestionCapsule`](../-sparql-question-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [filter](filter.md) | Decides whether to transform or not.`fun filter(input: `[`QuestionMessageCapsule`](../-question-message-capsule/index.md)`, context: `[`TransformationContext`](../../io.anima.transform/-transformation-context/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [transform](transform.md) | Transforms the input to some output.`fun transform(input: `[`QuestionMessageCapsule`](../-question-message-capsule/index.md)`, outputPromise: Promise<`[`SparqlQuestionCapsule`](../-sparql-question-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
