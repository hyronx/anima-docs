[anima](../../index.md) / [io.anima](../index.md) / [RuleLoaderVerticle](./index.md)

# RuleLoaderVerticle

`class RuleLoaderVerticle : `[`TransformationVerticle`](../../io.anima.transform/-transformation-verticle/index.md)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, `[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `RuleLoaderVerticle(ruleClass: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<out `[`Rule`](../../io.anima.graph/-rule/index.md)`>)` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | The input type for this transformation`val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>` |
| [name](name.md) | The name of this transformation`val name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [outputType](output-type.md) | The output type for this transformation`val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |
| [transform](transform.md) | Transforms the input to some output.`fun transform(input: `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, outputPromise: Promise<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../with.md) | `infix fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.with(state: `[`VerticleState`](../-verticle-state/index.md)`): `[`VerticleWithState`](../-verticle-with-state/index.md) |
