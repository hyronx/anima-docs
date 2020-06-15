[anima](../../index.md) / [io.anima](../index.md) / [ServiceType](./index.md)

# ServiceType

`sealed class ServiceType : `[`AnimaRessourceIdentifier`](../-anima-ressource-identifier/index.md)

### Types

| Name | Summary |
|---|---|
| [Cache](-cache.md) | `object Cache : `[`ServiceType`](./index.md) |
| [Custom](-custom/index.md) | `class Custom : `[`ServiceType`](./index.md) |
| [Gremlin](-gremlin.md) | `object Gremlin : `[`ServiceType`](./index.md) |
| [Http](-http.md) | `object Http : `[`ServiceType`](./index.md) |
| [Https](-https.md) | `object Https : `[`ServiceType`](./index.md) |
| [Transformation](-transformation/index.md) | `class Transformation<A : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`, B : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`> : `[`ServiceType`](./index.md) |

### Functions

| Name | Summary |
|---|---|
| [isRequirementMetBy](is-requirement-met-by.md) | `open fun isRequirementMetBy(others: `[`Iterable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-iterable/index.html)`<`[`ServiceType`](./index.md)`>): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [minusAssign](minus-assign.md) | `operator fun minusAssign(customServiceType: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [plusAssign](plus-assign.md) | `operator fun plusAssign(customServiceType: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [valueOf](value-of.md) | `fun valueOf(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`ServiceType`](./index.md)`?` |
