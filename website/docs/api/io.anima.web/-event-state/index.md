[anima](../../index.md) / [io.anima.web](../index.md) / [EventState](./index.md)

# EventState

`interface EventState : `[`Immutable`](../../io.anima.transform/-immutable/index.md)

### Properties

| Name | Summary |
|---|---|
| [event](event.md) | `abstract val event: BridgeEvent` |
| [eventType](event-type.md) | `abstract val eventType: BridgeEventType` |

### Inheritors

| Name | Summary |
|---|---|
| [IncomingEvent](../-incoming-event/index.md) | `sealed class IncomingEvent : `[`EventState`](./index.md) |
| [OutgoingEvent](../-outgoing-event/index.md) | `sealed class OutgoingEvent : `[`EventState`](./index.md) |
