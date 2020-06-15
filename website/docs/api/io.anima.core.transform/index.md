[anima](../index.md) / [io.anima.core.transform](./index.md)

## Package io.anima.core.transform

### Types

| Name | Summary |
|---|---|
| [AnimaGraphTimestampExtender](-anima-graph-timestamp-extender/index.md) | `class AnimaGraphTimestampExtender : `[`TransformationVerticle`](../io.anima.transform/-transformation-verticle/index.md)`<`[`AnimaGraphCapsule`](../io.anima.transform/-anima-graph-capsule/index.md)`, `[`ExtendedAnimaGraphCapsule`](../io.anima.transform/-extended-anima-graph-capsule/index.md)`>` |
| [AnswersCapsule](-answers-capsule/index.md) | `data class AnswersCapsule : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [GraphStoreCapsule](-graph-store-capsule/index.md) | `data class GraphStoreCapsule : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [GraphStoreRead](-graph-store-read.md) | `object GraphStoreRead : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [GremlinGraphSink](-gremlin-graph-sink/index.md) | Stores the input in a local Gremlin database.`class GremlinGraphSink : `[`SideEffect`](../io.anima.transform/-side-effect/index.md)`<`[`ExtendedAnimaGraphCapsule`](../io.anima.transform/-extended-anima-graph-capsule/index.md)`>` |
| [QuestionCapsule](-question-capsule/index.md) | `abstract class QuestionCapsule : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [QuestionMessageCapsule](-question-message-capsule/index.md) | `data class QuestionMessageCapsule : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [SequenceAnswersCapsule](-sequence-answers-capsule/index.md) | `data class SequenceAnswersCapsule : `[`SequenceCapsule`](../io.anima.transform/-sequence-capsule/index.md)`<`[`AnswersCapsule`](-answers-capsule/index.md)`>` |
| [SparqlQuestionCapsule](-sparql-question-capsule/index.md) | `data class SparqlQuestionCapsule : `[`QuestionCapsule`](-question-capsule/index.md) |
| [SparqlQuestionMessageTransformation](-sparql-question-message-transformation/index.md) | Transforms question messages to SPARQL questions for the transformation system if possible.`class SparqlQuestionMessageTransformation : `[`Transformation`](../io.anima.transform/-transformation/index.md)`<`[`QuestionMessageCapsule`](-question-message-capsule/index.md)`, `[`SparqlQuestionCapsule`](-sparql-question-capsule/index.md)`>` |
| [SparqlQuestionTransformation](-sparql-question-transformation/index.md) | `class SparqlQuestionTransformation : `[`Transformation`](../io.anima.transform/-transformation/index.md)`<`[`SparqlQuestionCapsule`](-sparql-question-capsule/index.md)`, `[`SequenceAnswersCapsule`](-sequence-answers-capsule/index.md)`>` |

### Extensions for External Classes

| Name | Summary |
|---|---|
| [io.vertx.core.json.JsonObject](io.vertx.core.json.-json-object/index.md) |  |
