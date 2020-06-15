[anima](../../index.md) / [io.anima.core](../index.md) / [QuestionToTransformationVerticle](./index.md)

# QuestionToTransformationVerticle

`class QuestionToTransformationVerticle : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)

Receives questions messages and transforms them to answers using the transformation system.

This class is a gateway for question messages to the transformation system.
In the future when the transformation system is directly address through [Address.TransformationRequested](../../io.anima/-address/-transformation-requested.md),
you won't need this class anymore. For this reason it must already be loaded as a module like this
in the config:

``` yaml
# config stuff before
modules:
  - provider: io.anima.core.QuestionToTransformationVerticle
    name: questionToTrafo
  # other modules
```

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Receives questions messages and transforms them to answers using the transformation system.`QuestionToTransformationVerticle()` |

### Functions

| Name | Summary |
|---|---|
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../../io.anima/-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |
| [start](start.md) | Configures and sets up this verticle.`fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |
