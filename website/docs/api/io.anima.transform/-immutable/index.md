[anima](../../index.md) / [io.anima.transform](../index.md) / [Immutable](./index.md)

# Immutable

`interface Immutable : `[`Cloneable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-cloneable/index.html)`, `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, `[`JsonObjectSerializable`](../../io.anima/-json-object-serializable/index.md)

Represents an immutable, serializable and cloneable type.

One requirement is the ability to be serializable to and from JSON.

In most cases you will want to create a wrapper with it for some other type
but make sure, your implementation still confirms to the aforementioned
conditions.

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns a JSON representation`open fun toJsonObject(): JsonObject` |

### Companion Object Properties

| Name | Summary |
|---|---|
| [objectMapper](object-mapper.md) | The commonly used [ObjectMapper](#) instance in this companion object`val objectMapper: ObjectMapper` |

### Companion Object Functions

| Name | Summary |
|---|---|
| [fromJsonBytes](from-json-bytes.md) | Converts [bytes](from-json-bytes.md#io.anima.transform.Immutable.Companion$fromJsonBytes(kotlin.ByteArray, java.lang.Class((io.anima.transform.Immutable.Companion.fromJsonBytes.T)))/bytes) to an [Immutable](./index.md) implementation as [type](from-json-bytes.md#io.anima.transform.Immutable.Companion$fromJsonBytes(kotlin.ByteArray, java.lang.Class((io.anima.transform.Immutable.Companion.fromJsonBytes.T)))/type).`fun <T : `[`Immutable`](./index.md)`> fromJsonBytes(bytes: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, type: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<T>): T!`<br>Converts [bytes](from-json-bytes.md#io.anima.transform.Immutable.Companion$fromJsonBytes(kotlin.ByteArray)/bytes) to an [Immutable](./index.md) implementation as type [T](from-json-bytes.md#T).`fun <T : `[`Immutable`](./index.md)`> fromJsonBytes(bytes: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`): T!` |
| [fromJsonObject](from-json-object.md) | Converts [json](from-json-object.md#io.anima.transform.Immutable.Companion$fromJsonObject(io.vertx.core.json.JsonObject, java.lang.Class((io.anima.transform.Immutable.Companion.fromJsonObject.T)))/json) to an [Immutable](./index.md) implementation as [type](from-json-object.md#io.anima.transform.Immutable.Companion$fromJsonObject(io.vertx.core.json.JsonObject, java.lang.Class((io.anima.transform.Immutable.Companion.fromJsonObject.T)))/type).`fun <T : `[`Immutable`](./index.md)`> fromJsonObject(json: JsonObject, type: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<T>): T!`<br>Converts [json](from-json-object.md#io.anima.transform.Immutable.Companion$fromJsonObject(io.vertx.core.json.JsonObject)/json) to an [Immutable](./index.md) implementation as type [T](from-json-object.md#T).`fun <T : `[`Immutable`](./index.md)`> fromJsonObject(json: JsonObject): T!` |

### Inheritors

| Name | Summary |
|---|---|
| [AnimaGraphCapsule](../-anima-graph-capsule/index.md) | `data class AnimaGraphCapsule : `[`Immutable`](./index.md) |
| [AnimaRessourceIdentifier](../../io.anima/-anima-ressource-identifier/index.md) | `open class AnimaRessourceIdentifier : `[`Immutable`](./index.md) |
| [AnswersCapsule](../../io.anima.core.transform/-answers-capsule/index.md) | `data class AnswersCapsule : `[`Immutable`](./index.md) |
| [DrawIoGraphCapsule](../-draw-io-graph-capsule/index.md) | `data class DrawIoGraphCapsule : `[`Immutable`](./index.md) |
| [DrawIoInput](../-draw-io-input/index.md) | `data class DrawIoInput : `[`Immutable`](./index.md) |
| [ExtendedAnimaGraphCapsule](../-extended-anima-graph-capsule/index.md) | `data class ExtendedAnimaGraphCapsule : `[`Immutable`](./index.md) |
| [GraphStoreCapsule](../../io.anima.core.transform/-graph-store-capsule/index.md) | `data class GraphStoreCapsule : `[`Immutable`](./index.md) |
| [GraphStoreRead](../../io.anima.core.transform/-graph-store-read.md) | `object GraphStoreRead : `[`Immutable`](./index.md) |
| [QuestionCapsule](../../io.anima.core.transform/-question-capsule/index.md) | `abstract class QuestionCapsule : `[`Immutable`](./index.md) |
| [QuestionMessageCapsule](../../io.anima.core.transform/-question-message-capsule/index.md) | `data class QuestionMessageCapsule : `[`Immutable`](./index.md) |
| [RdfGraph](../../io.anima.owl/-rdf-graph/index.md) | `data class RdfGraph : `[`Immutable`](./index.md) |
| [RdfInput](../../io.anima.owl/-rdf-input/index.md) | `sealed class RdfInput : `[`Immutable`](./index.md) |
| [ResultsCapsule](../-results-capsule/index.md) | `data class ResultsCapsule<T : `[`Immutable`](./index.md)`> : `[`Immutable`](./index.md) |
| [SequenceCapsule](../-sequence-capsule/index.md) | `abstract class SequenceCapsule<T : `[`Immutable`](./index.md)`> : `[`Immutable`](./index.md) |
| [StreamingCapsule](../-streaming-capsule/index.md) | `abstract class StreamingCapsule<T : `[`Immutable`](./index.md)`> : `[`Immutable`](./index.md) |
