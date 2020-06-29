[anima](../../index.md) / [io.anima.web](../index.md) / [OutgoingEvent](./index.md)

# OutgoingEvent

`sealed class OutgoingEvent : `[`EventState`](../-event-state/index.md)

### Properties

| Name | Summary |
|---|---|
| [destinations](destinations.md) | `abstract val destinations: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<SockJSSocket, `[`AnnouncementInfo`](../-announcement-info/index.md)`>` |
| [message](message.md) | `abstract val message: JsonObject` |

### Inheritors

| Name | Summary |
|---|---|
| [OutgoingClientEvent](../-outgoing-client-event/index.md) | `data class OutgoingClientEvent : `[`OutgoingEvent`](./index.md) |
| [OutgoingMindEvent](../-outgoing-mind-event/index.md) | `data class OutgoingMindEvent : `[`OutgoingEvent`](./index.md) |
