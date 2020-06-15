[anima](../../index.md) / [io.anima](../index.md) / [BasicAnimaVerticle](./index.md)

# BasicAnimaVerticle

`abstract class BasicAnimaVerticle : AbstractVerticle`

A very basic class for internal verticles in Anima only

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | A very basic class for internal verticles in Anima only`BasicAnimaVerticle()` |

### Properties

| Name | Summary |
|---|---|
| [configMap](config-map.md) | Not to be used right now`val ~~configMap~~: LocalMap<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`!, `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`!>` |
| [logger](logger.md) | The default logger instance which can be used by a subclassing verticle`open val logger: Logger` |
| [verticleName](verticle-name.md) | The verticle name as shown in e.g. logs`val verticleName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Functions

| Name | Summary |
|---|---|
| [toString](to-string.md) | The verticle string representation`open fun toString(): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [AnimaVerticle](../-anima-verticle/index.md) | The verticle base class for any verticle in Anima`abstract class AnimaVerticle : `[`BasicAnimaVerticle`](./index.md) |
| [ConfigVerticle](../../io.anima.core/-config-verticle/index.md) | `class ConfigVerticle : `[`BasicAnimaVerticle`](./index.md) |
| [HiveConnectionVerticle](../../io.anima.core/-hive-connection-verticle/index.md) | Establishes and manages a connection to one Hive.`class HiveConnectionVerticle : `[`BasicAnimaVerticle`](./index.md) |
| [MainVerticle](../../io.anima.core/-main-verticle/index.md) | `class MainVerticle : `[`BasicAnimaVerticle`](./index.md) |
