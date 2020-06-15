[anima](../../index.md) / [io.anima.transform](../index.md) / [Immutable](index.md) / [fromJsonBytes](./from-json-bytes.md)

# fromJsonBytes

`fun <T : `[`Immutable`](index.md)`> fromJsonBytes(bytes: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, type: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<T>): T!`

Converts [bytes](from-json-bytes.md#io.anima.transform.Immutable.Companion$fromJsonBytes(kotlin.ByteArray, java.lang.Class((io.anima.transform.Immutable.Companion.fromJsonBytes.T)))/bytes) to an [Immutable](index.md) implementation as [type](from-json-bytes.md#io.anima.transform.Immutable.Companion$fromJsonBytes(kotlin.ByteArray, java.lang.Class((io.anima.transform.Immutable.Companion.fromJsonBytes.T)))/type).

### Parameters

`bytes` - A byte array which must be readable as JSON

`type` - The type to convert the JSON to

**Return**
The converted type

`fun <reified T : `[`Immutable`](index.md)`> fromJsonBytes(bytes: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`): T!`

Converts [bytes](from-json-bytes.md#io.anima.transform.Immutable.Companion$fromJsonBytes(kotlin.ByteArray)/bytes) to an [Immutable](index.md) implementation as type [T](from-json-bytes.md#T).

### Parameters

`bytes` - A byte array which must be readable as JSON

**Return**
The converted type

