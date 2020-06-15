[anima](../../index.md) / [io.anima.core.mind](../index.md) / [MindVerticle](./index.md)

# MindVerticle

`class MindVerticle : `[`ModuleVerticle`](../../io.anima/-module-verticle/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `MindVerticle()` |

### Properties

| Name | Summary |
|---|---|
| [childVerticles](child-verticles.md) | `val childVerticles: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [mapDeploymentOptions](map-deployment-options.md) | `fun mapDeploymentOptions(currentConfig: JsonObject): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Pair`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-pair/index.html)`<DeploymentOptions, `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`>>` |
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../../io.anima/-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |
