[anima](../../index.md) / [io.anima](../index.md) / [DrawIoMainVerticle](./index.md)

# DrawIoMainVerticle

`class DrawIoMainVerticle : `[`AnimaVerticle`](../-anima-verticle/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `DrawIoMainVerticle()` |

### Functions

| Name | Summary |
|---|---|
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |
| [start](start.md) | Configures and sets up this verticle.`fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../with.md) | `infix fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.with(state: `[`VerticleState`](../-verticle-state/index.md)`): `[`VerticleWithState`](../-verticle-with-state/index.md) |
