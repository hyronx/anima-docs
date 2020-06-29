[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationVerticle](./index.md)

# TransformationVerticle

`abstract class TransformationVerticle<A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`, `[`Transformation`](../-transformation/index.md)`<A, B>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `TransformationVerticle(providedServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](../../io.anima/-service-type/index.md)`> = setOf())` |

### Properties

| Name | Summary |
|---|---|
| [logger](logger.md) | The default logger instance which can be used by a subclassing verticle`open val logger: Logger` |
| [providedServices](provided-services.md) | The provided services by this verticle`open val providedServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`ServiceType`](../../io.anima/-service-type/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [start](start.md) | Configures and sets up this verticle.`open fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [stop](stop.md) | Stops a Vert.x verticle.`open fun stop(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |

### Inheritors

| Name | Summary |
|---|---|
| [DrawIoGraphSourceVerticle](../-draw-io-graph-source-verticle/index.md) | `class DrawIoGraphSourceVerticle : `[`TransformationVerticle`](./index.md)`<`[`DrawIoInput`](../-draw-io-input/index.md)`, `[`DrawIoGraphCapsule`](../-draw-io-graph-capsule/index.md)`>` |
| [DrawIoGraphUnifierVerticle](../-draw-io-graph-unifier-verticle/index.md) | `class DrawIoGraphUnifierVerticle : `[`TransformationVerticle`](./index.md)`<`[`DrawIoGraphCapsule`](../-draw-io-graph-capsule/index.md)`, `[`AnimaGraphCapsule`](../-anima-graph-capsule/index.md)`>` |
