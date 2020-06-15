[anima](../../index.md) / [io.anima](../index.md) / [Address](./index.md)

# Address

`abstract class Address : `[`AnimaRessourceIdentifier`](../-anima-ressource-identifier/index.md)

Defines a event address

This address also is a [AnimaRessourceIdentifier](../-anima-ressource-identifier/index.md) (short ARI).
As that its format is as follows:
`anima:Address:<app>:<path>`
`<app>` should be replaced by a application or package name in reverse domain name form.
`<path>` is slash (`/`) separated path which has no special meaning.

An example of such ARI would be:
`anima:Address:io.anima.core:/config/update`
You should be able to confirm that with the following piece of code:
`println(Address.ConfigUpdate.toARI())`

[io.vertx.core.eventbus.MessageConsumer](#)s should listen to the full ARI.

### Types

| Name | Summary |
|---|---|
| [AnswerSend](-answer-send.md) | `object AnswerSend : CoreAddress` |
| [CacheDelete](-cache-delete.md) | `object CacheDelete : CoreAddress` |
| [CacheGet](-cache-get.md) | `object CacheGet : CoreAddress` |
| [CacheSave](-cache-save.md) | `object CacheSave : CoreAddress` |
| [ConfigUpdate](-config-update.md) | `object ConfigUpdate : CoreAddress` |
| [ConfigUpdated](-config-updated.md) | `object ConfigUpdated : CoreAddress` |
| [CoreAddress](-core-address/index.md) | `abstract class CoreAddress : `[`Address`](./index.md) |
| [ExportRequested](-export-requested.md) | `object ExportRequested : CoreAddress` |
| [ExportResult](-export-result.md) | `object ExportResult : CoreAddress` |
| [HiveRegistered](-hive-registered.md) | `object HiveRegistered : CoreAddress` |
| [HiveRequested](-hive-requested.md) | `object HiveRequested : CoreAddress` |
| [ImportStatus](-import-status.md) | `object ImportStatus : CoreAddress` |
| [NodeRegister](-node-register.md) | `object NodeRegister : CoreAddress` |
| [QuestionSend](-question-send.md) | `object QuestionSend : CoreAddress` |
| [TransformationRequested](-transformation-requested.md) | `object TransformationRequested : CoreAddress` |

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Defines a event address`Address(namespace: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`)` |

### Properties

| Name | Summary |
|---|---|
| [namespace](namespace.md) | Defines a application or package name`val namespace: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [path](path.md) | Defines some kind of path for an event`val path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [TransformationStatusAddress](../../io.anima.transform/-transformation-status-address/index.md) | The address where all status message related to the transformations of type [A](../../io.anima.transform/-transformation-status-address/index.md#A) to type [B](../../io.anima.transform/-transformation-status-address/index.md#B) can be received.`class TransformationStatusAddress<A : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`, B : `[`Immutable`](../../io.anima.transform/-immutable/index.md)`> : `[`Address`](./index.md) |
