[anima](../../index.md) / [io.anima](../index.md) / [MessagePackCodec](./index.md)

# MessagePackCodec

`class MessagePackCodec<R : `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`> : MessageCodec<R, R>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `MessagePackCodec(destinationType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<R>)` |

### Functions

| Name | Summary |
|---|---|
| [decodeFromWire](decode-from-wire.md) | `fun decodeFromWire(pos: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, buffer: Buffer): R` |
| [encodeToWire](encode-to-wire.md) | `fun encodeToWire(buffer: Buffer, s: R): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [name](name.md) | `fun name(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [systemCodecID](system-codec-i-d.md) | `fun systemCodecID(): `[`Byte`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte/index.html) |
| [transform](transform.md) | `fun transform(s: R): R` |
