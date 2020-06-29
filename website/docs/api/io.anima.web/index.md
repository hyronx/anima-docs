[anima](../index.md) / [io.anima.web](./index.md)

## Package io.anima.web

### Types

| Name | Summary |
|---|---|
| [AbstractWebVerticle](-abstract-web-verticle/index.md) | `abstract class AbstractWebVerticle : `[`AnimaVerticle`](../io.anima/-anima-verticle/index.md) |
| [AnnouncementInfo](-announcement-info/index.md) | `data class AnnouncementInfo : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [BridgeEventConsumer](-bridge-event-consumer.md) | `interface BridgeEventConsumer<A : `[`IncomingEvent`](-incoming-event/index.md)`> : `[`SideEffect`](../io.anima.transform/-side-effect/index.md)`<A>` |
| [BridgeEventHandler](-bridge-event-handler.md) | `interface BridgeEventHandler<A : `[`IncomingEvent`](-incoming-event/index.md)`, B : `[`OutgoingEvent`](-outgoing-event/index.md)`> : `[`Transformation`](../io.anima.transform/-transformation/index.md)`<A, B>` |
| [EventState](-event-state/index.md) | `interface EventState : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
| [IncomingClientEvent](-incoming-client-event/index.md) | `data class IncomingClientEvent : `[`IncomingEvent`](-incoming-event/index.md) |
| [IncomingEvent](-incoming-event/index.md) | `sealed class IncomingEvent : `[`EventState`](-event-state/index.md) |
| [IncomingMindEvent](-incoming-mind-event/index.md) | `data class IncomingMindEvent : `[`IncomingEvent`](-incoming-event/index.md) |
| [IncomingUnknownEvent](-incoming-unknown-event/index.md) | `data class IncomingUnknownEvent : `[`IncomingEvent`](-incoming-event/index.md) |
| [OutgoingClientEvent](-outgoing-client-event/index.md) | `data class OutgoingClientEvent : `[`OutgoingEvent`](-outgoing-event/index.md) |
| [OutgoingEvent](-outgoing-event/index.md) | `sealed class OutgoingEvent : `[`EventState`](-event-state/index.md) |
| [OutgoingMindEvent](-outgoing-mind-event/index.md) | `data class OutgoingMindEvent : `[`OutgoingEvent`](-outgoing-event/index.md) |
| [WebInput](-web-input/index.md) | `abstract class WebInput : `[`Immutable`](../io.anima.transform/-immutable/index.md) |
