[anima](../../index.md) / [io.anima](../index.md) / [RedisVerticle](./index.md)

# RedisVerticle

`class RedisVerticle : `[`ModuleVerticle`](../-module-verticle/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `RedisVerticle()` |

### Properties

| Name | Summary |
|---|---|
| [childVerticles](child-verticles.md) | `val childVerticles: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`RedisCacheVerticle`](../../io.anima.cache/-redis-cache-verticle/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../with.md) | `infix fun `[`AnimaVerticle`](../-anima-verticle/index.md)`.with(state: `[`VerticleState`](../-verticle-state/index.md)`): `[`VerticleWithState`](../-verticle-with-state/index.md) |
