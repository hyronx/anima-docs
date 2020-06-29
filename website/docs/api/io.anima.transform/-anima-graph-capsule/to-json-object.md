[anima](../../index.md) / [io.anima.transform](../index.md) / [AnimaGraphCapsule](index.md) / [toJsonObject](./to-json-object.md)

# toJsonObject

`fun toJsonObject(): JsonObject`

Returns a JSON representation

The default implementation uses the JacksonXML library for creating the [JsonObject](#).
You should only rely on it if your [Immutable](../-immutable/index.md) implementation just contains primitive transform types,
[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)s or [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)s. In most cases it's better to override this method.

**See Also**

[JsonObjectSerializable.toJsonObject](../../io.anima/-json-object-serializable/to-json-object.md)

**Return**
The [JsonObject](#) representation of this object

