[anima](../index.md) / [io.anima.identity](./index.md)

## Package io.anima.identity

### Types

| Name | Summary |
|---|---|
| [HumanIntelligence](-human-intelligence/index.md) | `class HumanIntelligence : `[`Identity`](-identity/index.md)`<`[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>` |
| [Identity](-identity/index.md) | `interface Identity<T : `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`> : `[`Principal`](https://docs.oracle.com/javase/6/docs/api/java/security/Principal.html) |
| [IdentityVerticle](-identity-verticle/index.md) | `class IdentityVerticle : `[`AnimaVerticle`](../io.anima/-anima-verticle/index.md) |
| [Signature](-signature/index.md) | `class Signature` |
| [Signer](-signer/index.md) | `interface Signer` |
| [TinkSigner](-tink-signer/index.md) | `class TinkSigner : `[`Signer`](-signer/index.md) |

### Functions

| Name | Summary |
|---|---|
| [sign](sign.md) | `fun <T : `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`> `[`Identity`](-identity/index.md)`<T>.sign(): `[`Signature`](-signature/index.md) |
