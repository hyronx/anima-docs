[anima](../../index.md) / [io.anima](../index.md) / [AnimaRessourceIdentifier](./index.md)

# AnimaRessourceIdentifier

`open class AnimaRessourceIdentifier : `[`Immutable`](../../io.anima.transform/-immutable/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `AnimaRessourceIdentifier(ressourceType: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, ressource: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`)` |

### Properties

| Name | Summary |
|---|---|
| [ressource](ressource.md) | `val ressource: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [ressourceType](ressource-type.md) | `val ressourceType: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [asURN](as-u-r-n.md) | `fun asURN(): URN` |
| [equals](equals.md) | `open fun equals(other: `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`?): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [hashCode](hash-code.md) | `open fun hashCode(): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
| [toHttpUrl](to-http-url.md) | `fun toHttpUrl(host: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "localhost", port: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)` = 10180): `[`URL`](https://docs.oracle.com/javase/6/docs/api/java/net/URL.html) |
| [toJsonObject](to-json-object.md) | Returns a JSON representation`open fun toJsonObject(): JsonObject` |
| [toString](to-string.md) | `open fun toString(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [toURL](to-u-r-l.md) | `fun toURL(): `[`URL`](https://docs.oracle.com/javase/6/docs/api/java/net/URL.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [create](create.md) | `fun create(ressourceType: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, ressource: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`AnimaRessourceIdentifier`](./index.md)<br>`fun create(ari: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`AnimaRessourceIdentifier`](./index.md)<br>`fun create(ari: `[`URI`](https://docs.oracle.com/javase/6/docs/api/java/net/URI.html)`): `[`AnimaRessourceIdentifier`](./index.md)<br>`fun create(ari: `[`URL`](https://docs.oracle.com/javase/6/docs/api/java/net/URL.html)`): `[`AnimaRessourceIdentifier`](./index.md) |

### Inheritors

| Name | Summary |
|---|---|
| [Address](../-address/index.md) | Defines a event address`abstract class Address : `[`AnimaRessourceIdentifier`](./index.md) |
| [ServiceType](../-service-type/index.md) | `sealed class ServiceType : `[`AnimaRessourceIdentifier`](./index.md) |
