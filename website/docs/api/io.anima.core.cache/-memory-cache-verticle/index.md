[anima](../../index.md) / [io.anima.core.cache](../index.md) / [MemoryCacheVerticle](./index.md)

# MemoryCacheVerticle

`class MemoryCacheVerticle : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`, `[`Cache`](../../io.anima.cache/-cache/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `MemoryCacheVerticle()` |

### Properties

| Name | Summary |
|---|---|
| [id](id.md) | `val id: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [get](get.md) | `fun get(key: `[`Ari`](../../io.anima/-ari.md)`): Future<JsonObject!>` |
| [getList](get-list.md) | `fun getList(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<JsonObject>!>` |
| [getSet](get-set.md) | `fun getSet(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<JsonObject>!>` |
| [has](has.md) | `fun has(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`!>` |
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../../io.anima/-anima-verticle/start.md) method.`fun processConfig(fullConfig: JsonObject): JsonObject` |
| [set](set.md) | `fun set(key: `[`Ari`](../../io.anima/-ari.md)`, value: JsonObject): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`!>` |
| [setList](set-list.md) | `fun setList(key: `[`Ari`](../../io.anima/-ari.md)`, value: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<JsonObject>): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`!>` |
| [setSet](set-set.md) | `fun setSet(key: `[`Ari`](../../io.anima/-ari.md)`, value: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<JsonObject>): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`!>` |
| [start](start.md) | Configures and sets up this verticle.`fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |
