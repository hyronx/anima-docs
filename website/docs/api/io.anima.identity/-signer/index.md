[anima](../../index.md) / [io.anima.identity](../index.md) / [Signer](./index.md)

# Signer

`interface Signer`

### Functions

| Name | Summary |
|---|---|
| [sign](sign.md) | `abstract fun sign(data: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`): `[`Signature`](../-signature/index.md) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun create(keyTemplate: KeyTemplate = SignatureKeyTemplates.ECDSA_P521): `[`Signer`](./index.md) |

### Inheritors

| Name | Summary |
|---|---|
| [TinkSigner](../-tink-signer/index.md) | `class TinkSigner : `[`Signer`](./index.md) |
