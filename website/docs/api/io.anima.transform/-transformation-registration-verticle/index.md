[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationRegistrationVerticle](./index.md)

# TransformationRegistrationVerticle

`class TransformationRegistrationVerticle<A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`, `[`Transformation`](../-transformation/index.md)`<A, B>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `TransformationRegistrationVerticle(transformation: `[`Transformation`](../-transformation/index.md)`<A, B>, providedServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](../../io.anima/-service-type/index.md)`> = setOf(
    ServiceType.Transformation(transformation.inputType, transformation.outputType)
  ))` |

### Properties

| Name | Summary |
|---|---|
| [logger](logger.md) | The default logger instance which can be used by a subclassing verticle`val logger: Logger` |
| [providedServices](provided-services.md) | The provided services by this verticle`val providedServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](../../io.anima/-service-type/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../../io.anima/-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |
| [start](start.md) | Configures and sets up this verticle.`fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [stop](stop.md) | Stops a Vert.x verticle.`fun stop(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |
