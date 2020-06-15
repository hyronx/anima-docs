[anima](../../index.md) / [io.anima.core.transform](../index.md) / [AnimaGraphTimestampExtender](./index.md)

# AnimaGraphTimestampExtender

`class AnimaGraphTimestampExtender : `[`TransformationVerticle`](../../io.anima.transform/-transformation-verticle/index.md)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, `[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `AnimaGraphTimestampExtender()` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | The input type for this transformation`val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`>` |
| [outputType](output-type.md) | The output type for this transformation`val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [filter](filter.md) | Decides whether to transform or not.`fun filter(input: `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, context: `[`TransformationContext`](../../io.anima.transform/-transformation-context/index.md)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../../io.anima/-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |
| [transform](transform.md) | Transforms the input to some output.`fun transform(input: `[`AnimaGraphCapsule`](../../io.anima.transform/-anima-graph-capsule/index.md)`, outputPromise: Promise<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |
