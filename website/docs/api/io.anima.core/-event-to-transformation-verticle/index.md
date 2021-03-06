[anima](../../index.md) / [io.anima.core](../index.md) / [EventToTransformationVerticle](./index.md)

# EventToTransformationVerticle

`class EventToTransformationVerticle : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `EventToTransformationVerticle()` |

### Functions

| Name | Summary |
|---|---|
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../../io.anima/-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |
| [start](start.md) | Configures and sets up this verticle.`fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |
