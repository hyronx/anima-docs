[anima](../../index.md) / [io.anima.web](../index.md) / [IncomingClientEvent](./index.md)

# IncomingClientEvent

`data class IncomingClientEvent : `[`IncomingEvent`](../-incoming-event/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `IncomingClientEvent(event: BridgeEvent, eventType: BridgeEventType = event.type(), source: SockJSSocket = event.socket())` |

### Properties

| Name | Summary |
|---|---|
| [event](event.md) | `val event: BridgeEvent` |
| [eventType](event-type.md) | `val eventType: BridgeEventType` |
| [source](source.md) | `val source: SockJSSocket` |

### Functions

| Name | Summary |
|---|---|
| [transition](transition.md) | `fun transition(destinations: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<SockJSSocket, `[`AnnouncementInfo`](../-announcement-info/index.md)`>): `[`OutgoingEvent`](../-outgoing-event/index.md) |
