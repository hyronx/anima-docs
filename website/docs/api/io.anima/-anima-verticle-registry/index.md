[anima](../../index.md) / [io.anima](../index.md) / [AnimaVerticleRegistry](./index.md)

# AnimaVerticleRegistry

`object AnimaVerticleRegistry`

### Properties

| Name | Summary |
|---|---|
| [verticlesSortedByDependencies](verticles-sorted-by-dependencies.md) | `val verticlesSortedByDependencies: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`AnimaVerticle`](../-anima-verticle/index.md)`>` |
| [verticlesWithState](verticles-with-state.md) | `val verticlesWithState: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`VerticleWithState`](../-verticle-with-state/index.md)`!>` |

### Functions

| Name | Summary |
|---|---|
| [canStart](can-start.md) | `fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.canStart(): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [getVerticle](get-verticle.md) | `fun getVerticle(verticle: `[`AnimaVerticle`](../-anima-verticle/index.md)`): `[`VerticleWithState`](../-verticle-with-state/index.md)`?` |
| [getVerticleByName](get-verticle-by-name.md) | `fun <T : `[`AnimaVerticle`](../-anima-verticle/index.md)`> getVerticleByName(verticleName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): T?` |
| [getVerticlesByService](get-verticles-by-service.md) | `fun getVerticlesByService(serviceType: `[`ServiceType`](../-service-type/index.md)`): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`AnimaVerticle`](../-anima-verticle/index.md)`>?`<br>`fun getVerticlesByService(serviceTypeName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`AnimaVerticle`](../-anima-verticle/index.md)`>?` |
| [remove](remove.md) | `fun `[`VerticleStateHandler`](../-verticle-state-handler.md)`.remove(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [setDisabled](set-disabled.md) | `fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.setDisabled(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [setQueued](set-queued.md) | `fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.setQueued(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [setStarted](set-started.md) | `fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.setStarted(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [setStarting](set-starting.md) | `fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.setStarting(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [setStopped](set-stopped.md) | `fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.setStopped(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [setWantStart](set-want-start.md) | `fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.setWantStart(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [stateHandler](state-handler.md) | `fun stateHandler(handler: `[`VerticleStateHandler`](../-verticle-state-handler.md)`): `[`VerticleStateHandler`](../-verticle-state-handler.md) |
