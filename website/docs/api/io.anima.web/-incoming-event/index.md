[anima](../../index.md) / [io.anima.web](../index.md) / [IncomingEvent](./index.md)

# IncomingEvent

`sealed class IncomingEvent : `[`EventState`](../-event-state/index.md)

### Properties

| Name | Summary |
|---|---|
| [source](source.md) | `abstract val source: SockJSSocket` |

### Functions

| Name | Summary |
|---|---|
| [transition](transition.md) | `abstract fun transition(destinations: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<SockJSSocket, `[`AnnouncementInfo`](../-announcement-info/index.md)`>): `[`OutgoingEvent`](../-outgoing-event/index.md) |

### Inheritors

| Name | Summary |
|---|---|
| [IncomingClientEvent](../-incoming-client-event/index.md) | `data class IncomingClientEvent : `[`IncomingEvent`](./index.md) |
| [IncomingMindEvent](../-incoming-mind-event/index.md) | `data class IncomingMindEvent : `[`IncomingEvent`](./index.md) |
| [IncomingUnknownEvent](../-incoming-unknown-event/index.md) | `data class IncomingUnknownEvent : `[`IncomingEvent`](./index.md) |
