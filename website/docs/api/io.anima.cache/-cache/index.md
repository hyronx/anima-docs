[anima](../../index.md) / [io.anima.cache](../index.md) / [Cache](./index.md)

# Cache

`interface Cache`

### Types

| Name | Summary |
|---|---|
| [Companion](-companion/index.md) | `companion object Companion : `[`Cache`](./index.md) |

### Properties

| Name | Summary |
|---|---|
| [id](id.md) | `abstract val id: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [get](get.md) | `abstract fun get(key: `[`Ari`](../../io.anima/-ari.md)`): Future<JsonObject>` |
| [getList](get-list.md) | `abstract fun getList(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<JsonObject>>` |
| [getSet](get-set.md) | `abstract fun getSet(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<JsonObject>>` |
| [has](has.md) | `abstract fun has(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>` |
| [set](set.md) | `abstract fun set(key: `[`Ari`](../../io.anima/-ari.md)`, value: JsonObject): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>` |
| [setList](set-list.md) | `abstract fun setList(key: `[`Ari`](../../io.anima/-ari.md)`, value: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<JsonObject>): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>` |
| [setSet](set-set.md) | `abstract fun setSet(key: `[`Ari`](../../io.anima/-ari.md)`, value: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<JsonObject>): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>` |

### Companion Object Properties

| Name | Summary |
|---|---|
| [id](id.md) | `val id: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [get](get.md) | `fun get(key: `[`Ari`](../../io.anima/-ari.md)`): Future<JsonObject>` |
| [getList](get-list.md) | `fun getList(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<JsonObject>>` |
| [getSet](get-set.md) | `fun getSet(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<JsonObject>>` |
| [has](has.md) | `fun has(key: `[`Ari`](../../io.anima/-ari.md)`): Future<`[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`>` |
| [set](set.md) | `fun set(key: `[`Ari`](../../io.anima/-ari.md)`, value: JsonObject): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>` |
| [setList](set-list.md) | `fun setList(key: `[`Ari`](../../io.anima/-ari.md)`, value: `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<JsonObject>): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>` |
| [setSet](set-set.md) | `fun setSet(key: `[`Ari`](../../io.anima/-ari.md)`, value: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<JsonObject>): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>` |

### Inheritors

| Name | Summary |
|---|---|
| [MemoryCacheVerticle](../../io.anima.core.cache/-memory-cache-verticle/index.md) | `class MemoryCacheVerticle : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`, `[`Cache`](./index.md) |
| [RedisCacheVerticle](../-redis-cache-verticle/index.md) | `class RedisCacheVerticle : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`, `[`Cache`](./index.md) |
