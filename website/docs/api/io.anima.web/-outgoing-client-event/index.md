[anima](../../index.md) / [io.anima.web](../index.md) / [OutgoingClientEvent](./index.md)

# OutgoingClientEvent

`data class OutgoingClientEvent : `[`OutgoingEvent`](../-outgoing-event/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `OutgoingClientEvent(event: BridgeEvent, destination: `[`Pair`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-pair/index.html)`<SockJSSocket, `[`AnnouncementInfo`](../-announcement-info/index.md)`>, eventType: BridgeEventType = event.type(), message: JsonObject = event.rawMessage)` |

### Properties

| Name | Summary |
|---|---|
| [destination](destination.md) | `val destination: `[`Pair`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-pair/index.html)`<SockJSSocket, `[`AnnouncementInfo`](../-announcement-info/index.md)`>` |
| [destinations](destinations.md) | `val destinations: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<SockJSSocket, `[`AnnouncementInfo`](../-announcement-info/index.md)`>` |
| [event](event.md) | `val event: BridgeEvent` |
| [eventType](event-type.md) | `val eventType: BridgeEventType` |
| [message](message.md) | `val message: JsonObject` |
