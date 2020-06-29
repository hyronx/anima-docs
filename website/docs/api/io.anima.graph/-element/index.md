[anima](../../index.md) / [io.anima.graph](../index.md) / [Element](./index.md)

# Element

`sealed class Element : `[`Immutable`](../../io.anima.transform/-immutable/index.md)

### Properties

| Name | Summary |
|---|---|
| [javaType](java-type.md) | `abstract val javaType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<*>` |
| [layer](layer.md) | `abstract val layer: `[`Layer`](../-layer/index.md) |
| [value](value.md) | `abstract val value: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html) |

### Functions

| Name | Summary |
|---|---|
| [equals](equals.md) | `open fun equals(other: `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`?): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [hashCode](hash-code.md) | `open fun hashCode(): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
| [toJsonObject](to-json-object.md) | Returns a JSON representation`open fun toJsonObject(): JsonObject` |

### Inheritors

| Name | Summary |
|---|---|
| [Edge](../-edge/index.md) | `class Edge : `[`Element`](./index.md) |
| [Vertex](../-vertex/index.md) | `class Vertex : `[`Element`](./index.md) |
