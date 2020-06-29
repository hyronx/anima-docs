[anima](../../index.md) / [io.anima.transform](../index.md) / [SequenceCapsule](./index.md)

# SequenceCapsule

`abstract class SequenceCapsule<T : `[`Immutable`](../-immutable/index.md)`> : `[`Immutable`](../-immutable/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `SequenceCapsule()` |

### Properties

| Name | Summary |
|---|---|
| [sequence](sequence.md) | `abstract val sequence: `[`Sequence`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.sequences/-sequence/index.html)`<T>` |
| [type](type.md) | `abstract val type: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<T>` |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns a JSON representation`open fun toJsonObject(): JsonObject` |

### Inheritors

| Name | Summary |
|---|---|
| [SequenceAnswersCapsule](../../io.anima.messages/-sequence-answers-capsule/index.md) | `data class SequenceAnswersCapsule : `[`SequenceCapsule`](./index.md)`<`[`AnswersCapsule`](../../io.anima.messages/-answers-capsule/index.md)`>` |
