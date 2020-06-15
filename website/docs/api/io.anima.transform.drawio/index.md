[anima](../index.md) / [io.anima.transform.drawio](./index.md)

## Package io.anima.transform.drawio

### Types

| Name | Summary |
|---|---|
| [Cell](-cell/index.md) | `sealed class Cell` |
| [Graph](-graph/index.md) | `data class Graph` |
| [GraphParts](-graph-parts/index.md) | `data class GraphParts` |
| [LayerMap](-layer-map/index.md) | `data class LayerMap` |
| [MetaGraphParts](-meta-graph-parts/index.md) | `data class MetaGraphParts` |
| [XmlEventHandler](-xml-event-handler/index.md) | `class XmlEventHandler : `[`DefaultHandler`](https://docs.oracle.com/javase/6/docs/api/org/xml/sax/helpers/DefaultHandler.html) |

### Exceptions

| Name | Summary |
|---|---|
| [DrawIoGraphConnectionException](-draw-io-graph-connection-exception/index.md) | `class DrawIoGraphConnectionException : `[`RuntimeException`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-runtime-exception/index.html) |
| [DrawIoXmlParserException](-draw-io-xml-parser-exception/index.md) | `class DrawIoXmlParserException : `[`RuntimeException`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-runtime-exception/index.html) |

### Functions

| Name | Summary |
|---|---|
| [get](get.md) | `operator fun `[`LayerMap`](-layer-map/index.md)`.get(layer: `[`Layer`](../io.anima.graph/-layer/index.md)`): `[`MutableList`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-mutable-list/index.html)`<`[`Cell`](-cell/index.md)`>` |
| [removeIf](remove-if.md) | `fun `[`LayerMap`](-layer-map/index.md)`.removeIf(finder: (`[`Cell`](-cell/index.md)`) -> `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [toDrawIoGraph](to-draw-io-graph.md) | `fun `[`LayerMap`](-layer-map/index.md)`.toDrawIoGraph(): `[`Graph`](-graph/index.md) |
