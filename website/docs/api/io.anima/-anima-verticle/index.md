[anima](../../index.md) / [io.anima](../index.md) / [AnimaVerticle](./index.md)

# AnimaVerticle

`abstract class AnimaVerticle : `[`BasicAnimaVerticle`](../-basic-anima-verticle/index.md)

The verticle base class for any verticle in Anima

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | The verticle base class for any verticle in Anima`AnimaVerticle()` |

### Properties

| Name | Summary |
|---|---|
| [deploymentOptions](deployment-options.md) | The default deployment options to be used for this verticle`open val deploymentOptions: DeploymentOptions?` |
| [providedServices](provided-services.md) | The provided services by this verticle`open val providedServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](../-service-type/index.md)`>` |
| [requiredServices](required-services.md) | The required services by this verticle which have to be available before startup`open val requiredServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](../-service-type/index.md)`>` |
| [requiresServices](requires-services.md) | Gives information whether this verticle requires any services`val requiresServices: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |

### Functions

| Name | Summary |
|---|---|
| [afterStart](after-start.md) | Gets called after [start](start.md) has finished.`open fun afterStart(firstConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [beforeStart](before-start.md) | Gets called before [start](start.md) is called.`open fun beforeStart(firstConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [checkHealth](check-health.md) | Returns health information for this verticle`open fun checkHealth(statusPromise: Promise<Status>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [deployChildTransformation](deploy-child-transformation.md) | Deploys a child transformation`fun deployChildTransformation(transformation: `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<*, *>, deploymentOptions: DeploymentOptions = deploymentOptionsOf()): Future<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`!>` |
| [deployChildTransformations](deploy-child-transformations.md) | Deploys child transformations`fun deployChildTransformations(transformations: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Transformation`](../../io.anima.transform/-transformation/index.md)`<*, *>>, deploymentOptions: DeploymentOptions = deploymentOptionsOf()): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<Future<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>>` |
| [handleDeploymentResult](handle-deployment-result.md) | Returns a handler for the deployment result of a child verticle.`open fun <A : `[`AnimaVerticle`](./index.md)`> handleDeploymentResult(childClass: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, promise: Promise<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>): (AsyncResult<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>`fun <A : `[`AnimaVerticle`](./index.md)`> handleDeploymentResult(promise: Promise<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>): (AsyncResult<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](start.md) method.`abstract fun processConfig(fullConfig: JsonObject): JsonObject` |
| [start](start.md) | Configures and sets up this verticle.`abstract fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Starts a Vert.x verticle.`open fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [stop](stop.md) | Stops a Vert.x verticle.`open fun stop(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [updateConfig](update-config.md) | Updates the configuration with the new one.`fun JsonObject.updateConfig(newFullConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../with.md) | `infix fun `[`AnimaVerticle`](./index.md)`.with(state: `[`VerticleState`](../-verticle-state/index.md)`): `[`VerticleWithState`](../-verticle-with-state/index.md) |

### Inheritors

| Name | Summary |
|---|---|
| [AbstractWebVerticle](../../io.anima.core.web/-abstract-web-verticle/index.md) | `abstract class AbstractWebVerticle : `[`AnimaVerticle`](./index.md) |
| [DataManagerVerticle](../../io.anima.core.mind/-data-manager-verticle/index.md) | `class DataManagerVerticle : `[`AnimaVerticle`](./index.md) |
| [DrawIoMainVerticle](../-draw-io-main-verticle/index.md) | `class DrawIoMainVerticle : `[`AnimaVerticle`](./index.md) |
| [EventToTransformationVerticle](../../io.anima.core/-event-to-transformation-verticle/index.md) | `class EventToTransformationVerticle : `[`AnimaVerticle`](./index.md) |
| [GraphStoreVerticle](../../io.anima.core.store/-graph-store-verticle/index.md) | `class GraphStoreVerticle : `[`AnimaVerticle`](./index.md) |
| [GremlinVerticle](../../io.anima.core.mind/-gremlin-verticle/index.md) | `class GremlinVerticle : `[`AnimaVerticle`](./index.md) |
| [HiveClientVerticle](../../io.anima.core/-hive-client-verticle/index.md) | `class HiveClientVerticle : `[`AnimaVerticle`](./index.md) |
| [IdentityVerticle](../../io.anima.identity/-identity-verticle/index.md) | `class IdentityVerticle : `[`AnimaVerticle`](./index.md) |
| [MemoryCacheVerticle](../../io.anima.core.cache/-memory-cache-verticle/index.md) | `class MemoryCacheVerticle : `[`AnimaVerticle`](./index.md)`, `[`Cache`](../../io.anima.cache/-cache/index.md) |
| [ModuleVerticle](../-module-verticle/index.md) | `abstract class ModuleVerticle : `[`AnimaVerticle`](./index.md) |
| [OwlMainVerticle](../../io.anima.owl/-owl-main-verticle/index.md) | `class OwlMainVerticle : `[`AnimaVerticle`](./index.md) |
| [QuestionToTransformationVerticle](../../io.anima.core/-question-to-transformation-verticle/index.md) | Receives questions messages and transforms them to answers using the transformation system.`class QuestionToTransformationVerticle : `[`AnimaVerticle`](./index.md) |
| [RedisCacheVerticle](../../io.anima.cache/-redis-cache-verticle/index.md) | `class RedisCacheVerticle : `[`AnimaVerticle`](./index.md)`, `[`Cache`](../../io.anima.cache/-cache/index.md) |
| [RedisVerticle](../-redis-verticle/index.md) | `class RedisVerticle : `[`AnimaVerticle`](./index.md) |
| [RulesVerticle](../-rules-verticle/index.md) | `class RulesVerticle : `[`AnimaVerticle`](./index.md) |
| [TransformationRegistrationVerticle](../../io.anima.transform/-transformation-registration-verticle/index.md) | `class TransformationRegistrationVerticle<A : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`, B : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`> : `[`AnimaVerticle`](./index.md)`, `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<A, B>` |
| [TransformationVerticle](../../io.anima.transform/-transformation-verticle/index.md) | `abstract class TransformationVerticle<A : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`, B : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`> : `[`AnimaVerticle`](./index.md)`, `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<A, B>` |
