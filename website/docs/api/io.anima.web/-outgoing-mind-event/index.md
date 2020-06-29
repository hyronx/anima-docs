[anima](../../index.md) / [io.anima.web](../index.md) / [OutgoingMindEvent](./index.md)

# OutgoingMindEvent

`data class OutgoingMindEvent : `[`OutgoingEvent`](../-outgoing-event/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `OutgoingMindEvent(event: BridgeEvent, destinations: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<SockJSSocket, `[`AnnouncementInfo`](../-announcement-info/index.md)`>, eventType: BridgeEventType = event.type(), message: JsonObject = event.rawMessage)` |

### Properties

| Name | Summary |
|---|---|
| [destinations](destinations.md) | `val destinations: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<SockJSSocket, `[`AnnouncementInfo`](../-announcement-info/index.md)`>` |
| [event](event.md) | `val event: BridgeEvent` |
| [eventType](event-type.md) | `val eventType: BridgeEventType` |
| [message](message.md) | `val message: JsonObject` |
