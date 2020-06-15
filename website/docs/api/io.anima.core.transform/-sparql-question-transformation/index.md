[anima](../../index.md) / [io.anima.core.transform](../index.md) / [SparqlQuestionTransformation](./index.md)

# SparqlQuestionTransformation

`class SparqlQuestionTransformation : `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`SparqlQuestionCapsule`](../-sparql-question-capsule/index.md)`, `[`SequenceAnswersCapsule`](../-sequence-answers-capsule/index.md)`>`

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | The input type for this transformation`val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`SparqlQuestionCapsule`](../-sparql-question-capsule/index.md)`>` |
| [outputType](output-type.md) | The output type for this transformation`val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`SequenceAnswersCapsule`](../-sequence-answers-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [transform](transform.md) | Transforms the input to some output.`fun transform(input: `[`SparqlQuestionCapsule`](../-sparql-question-capsule/index.md)`, outputPromise: Promise<`[`SequenceAnswersCapsule`](../-sequence-answers-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun create(vertx: Vertx, traversal: SparqlTraversalSource): `[`SparqlQuestionTransformation`](./index.md) |
