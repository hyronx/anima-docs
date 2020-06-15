[anima](../index.md) / [io.anima](./index.md)

## Package io.anima

### Types

| Name | Summary |
|---|---|
| [Address](-address/index.md) | Defines a event address`abstract class Address : `[`AnimaRessourceIdentifier`](-anima-ressource-identifier/index.md) |
| [AnimaRessourceIdentifier](-anima-ressource-identifier/index.md) | `open class AnimaRessourceIdentifier : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [AnimaType](-anima-type/index.md) | `sealed class AnimaType` |
| [AnimaVerticle](-anima-verticle/index.md) | The verticle base class for any verticle in Anima`abstract class AnimaVerticle : `[`BasicAnimaVerticle`](-basic-anima-verticle/index.md) |
| [AnimaVerticleRegistry](-anima-verticle-registry/index.md) | `object AnimaVerticleRegistry` |
| [Ari](-ari.md) | `typealias Ari = `[`AnimaRessourceIdentifier`](-anima-ressource-identifier/index.md) |
| [BasicAnimaVerticle](-basic-anima-verticle/index.md) | A very basic class for internal verticles in Anima only`abstract class BasicAnimaVerticle : AbstractVerticle` |
| [DrawIoMainVerticle](-draw-io-main-verticle/index.md) | `class DrawIoMainVerticle : `[`AnimaVerticle`](-anima-verticle/index.md) |
| [JsonObjectSerializable](-json-object-serializable/index.md) | Represents a JSON serializable object`interface JsonObjectSerializable` |
| [MessagePackCodec](-message-pack-codec/index.md) | `class MessagePackCodec<R : `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`> : MessageCodec<R, R>` |
| [ModuleVerticle](-module-verticle/index.md) | `abstract class ModuleVerticle : `[`AnimaVerticle`](-anima-verticle/index.md) |
| [RedisVerticle](-redis-verticle/index.md) | `class RedisVerticle : `[`AnimaVerticle`](-anima-verticle/index.md) |
| [RuleLoaderVerticle](-rule-loader-verticle/index.md) | `class RuleLoaderVerticle : `[`TransformationVerticle`](../io.anima.transform/-transformation-verticle/index.md)`<`[`AnimaGraphCapsule`](../io.anima.transform/-anima-graph-capsule/index.md)`, `[`ExtendedAnimaGraphCapsule`](../io.anima.transform/-extended-anima-graph-capsule/index.md)`>` |
| [RulesVerticle](-rules-verticle/index.md) | `class RulesVerticle : `[`AnimaVerticle`](-anima-verticle/index.md) |
| [ServiceType](-service-type/index.md) | `sealed class ServiceType : `[`AnimaRessourceIdentifier`](-anima-ressource-identifier/index.md) |
| [VerticleState](-verticle-state/index.md) | `enum class VerticleState` |
| [VerticleStateHandler](-verticle-state-handler.md) | `typealias VerticleStateHandler = (verticle: `[`AnimaVerticle`](-anima-verticle/index.md)`, state: `[`VerticleState`](-verticle-state/index.md)`) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [VerticleWithState](-verticle-with-state/index.md) | `data class VerticleWithState` |

### Extensions for External Classes

| Name | Summary |
|---|---|
| [io.vertx.core.eventbus.EventBus](io.vertx.core.eventbus.-event-bus/index.md) |  |
| [io.vertx.core.Promise](io.vertx.core.-promise/index.md) |  |
| [kotlin.collections.Iterable](kotlin.collections.-iterable/index.md) |  |
| [kotlin.collections.Map](kotlin.collections.-map/index.md) |  |
| [kotlin.collections.Set](kotlin.collections.-set/index.md) |  |

### Functions

| Name | Summary |
|---|---|
| [serviceTypesOf](service-types-of.md) | `fun serviceTypesOf(vararg serviceTypes: `[`ServiceType`](-service-type/index.md)`): `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](-service-type/index.md)`>` |
| [with](with.md) | `infix fun `[`AnimaVerticle`](-anima-verticle/index.md)`.with(state: `[`VerticleState`](-verticle-state/index.md)`): `[`VerticleWithState`](-verticle-with-state/index.md) |
