[anima](../../index.md) / [io.anima.transform](../index.md) / [DrawIoGraphSourceVerticle](./index.md)

# DrawIoGraphSourceVerticle

`class DrawIoGraphSourceVerticle : `[`TransformationVerticle`](../-transformation-verticle/index.md)`<`[`DrawIoInput`](../-draw-io-input/index.md)`, `[`DrawIoGraphCapsule`](../-draw-io-graph-capsule/index.md)`>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `DrawIoGraphSourceVerticle()` |

### Properties

| Name | Summary |
|---|---|
| [inputType](input-type.md) | The input type for this transformation`val inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`DrawIoInput`](../-draw-io-input/index.md)`>` |
| [outputType](output-type.md) | The output type for this transformation`val outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<`[`DrawIoGraphCapsule`](../-draw-io-graph-capsule/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../../io.anima/-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |
| [transform](transform.md) | Transforms the input to some output.`fun transform(input: `[`DrawIoInput`](../-draw-io-input/index.md)`, outputPromise: Promise<`[`DrawIoGraphCapsule`](../-draw-io-graph-capsule/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |
