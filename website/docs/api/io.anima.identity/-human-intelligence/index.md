[anima](../../index.md) / [io.anima.identity](../index.md) / [HumanIntelligence](./index.md)

# HumanIntelligence

`class HumanIntelligence : `[`Identity`](../-identity/index.md)`<`[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `HumanIntelligence(signer: `[`Signer`](../-signer/index.md)`, uuid: `[`UUID`](https://docs.oracle.com/javase/6/docs/api/java/util/UUID.html)` = UUID.randomUUID(), attributes: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>)` |

### Properties

| Name | Summary |
|---|---|
| [attributes](attributes.md) | `val attributes: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>` |
| [birthDate](birth-date.md) | `val birthDate: `[`Date`](https://docs.oracle.com/javase/6/docs/api/java/util/Date.html) |
| [firstName](first-name.md) | `val firstName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [lastName](last-name.md) | `val lastName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [schema](schema.md) | `val schema: HumanIntelligence` |
| [signature](signature.md) | `val signature: `[`Signature`](../-signature/index.md) |
| [signer](signer.md) | `val signer: `[`Signer`](../-signer/index.md) |
| [uuid](uuid.md) | `val uuid: `[`UUID`](https://docs.oracle.com/javase/6/docs/api/java/util/UUID.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [sign](../sign.md) | `fun <T : `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`> `[`Identity`](../-identity/index.md)`<T>.sign(): `[`Signature`](../-signature/index.md) |
