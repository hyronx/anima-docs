[anima](../../index.md) / [io.anima.identity](../index.md) / [Identity](./index.md)

# Identity

`interface Identity<T : `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`> : `[`Principal`](https://docs.oracle.com/javase/6/docs/api/java/security/Principal.html)

### Properties

| Name | Summary |
|---|---|
| [attributes](attributes.md) | `abstract val attributes: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, T>` |
| [schema](schema.md) | `abstract val schema: IdentityType` |
| [signature](signature.md) | `abstract val signature: `[`Signature`](../-signature/index.md) |
| [signer](signer.md) | `abstract val signer: `[`Signer`](../-signer/index.md) |
| [uuid](uuid.md) | `abstract val uuid: `[`UUID`](https://docs.oracle.com/javase/6/docs/api/java/util/UUID.html) |

### Functions

| Name | Summary |
|---|---|
| [getName](get-name.md) | `open fun getName(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [sign](../sign.md) | `fun <T : `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`> `[`Identity`](./index.md)`<T>.sign(): `[`Signature`](../-signature/index.md) |

### Inheritors

| Name | Summary |
|---|---|
| [HumanIntelligence](../-human-intelligence/index.md) | `class HumanIntelligence : `[`Identity`](./index.md)`<`[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>` |
