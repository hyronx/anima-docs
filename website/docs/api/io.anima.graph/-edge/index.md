[anima](../../index.md) / [io.anima.graph](../index.md) / [Edge](./index.md)

# Edge

`class Edge : `[`Element`](../-element/index.md)

### Properties

| Name | Summary |
|---|---|
| [javaType](java-type.md) | `val javaType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<*>` |
| [layer](layer.md) | `val layer: `[`Layer`](../-layer/index.md) |
| [value](value.md) | `val value: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html) |

### Functions

| Name | Summary |
|---|---|
| [toJsonObject](to-json-object.md) | Returns a JSON representation`fun toJsonObject(): JsonObject` |

### Companion Object Properties

| Name | Summary |
|---|---|
| [TYPE](-t-y-p-e.md) | `const val TYPE: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun create(layer: `[`Layer`](../-layer/index.md)`, value: `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, javaType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<*>): `[`Edge`](./index.md)<br>`fun <T : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`> create(layer: `[`Layer`](../-layer/index.md)`, value: T): `[`Edge`](./index.md) |
