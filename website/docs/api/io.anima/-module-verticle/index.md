[anima](../../index.md) / [io.anima](../index.md) / [ModuleVerticle](./index.md)

# ModuleVerticle

`abstract class ModuleVerticle : `[`AnimaVerticle`](../-anima-verticle/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `ModuleVerticle()` |

### Properties

| Name | Summary |
|---|---|
| [childVerticles](child-verticles.md) | `abstract val childVerticles: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`AnimaVerticle`](../-anima-verticle/index.md)`>` |
| [providedServices](provided-services.md) | The provided services by this verticle`open val providedServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](../-service-type/index.md)`>` |
| [requiredServices](required-services.md) | The required services by this verticle which have to be available before startup`open val requiredServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](../-service-type/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [mapDeploymentOptions](map-deployment-options.md) | `open fun mapDeploymentOptions(currentConfig: JsonObject): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Pair`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-pair/index.html)`<DeploymentOptions, `[`AnimaVerticle`](../-anima-verticle/index.md)`>>` |
| [start](start.md) | Configures and sets up this verticle.`open fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../with.md) | `infix fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.with(state: `[`VerticleState`](../-verticle-state/index.md)`): `[`VerticleWithState`](../-verticle-with-state/index.md) |

### Inheritors

| Name | Summary |
|---|---|
| [RedisVerticle](../-redis-verticle/index.md) | `class RedisVerticle : `[`ModuleVerticle`](./index.md) |
