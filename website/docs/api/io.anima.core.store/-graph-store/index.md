[anima](../../index.md) / [io.anima.core.store](../index.md) / [GraphStore](./index.md)

# GraphStore

`class GraphStore`

A graph representation divided in vertices, edges and triples

This [GraphStore](./index.md) class only is an internal representation
which is temporarily used to store the graph in [Graph](../../io.anima.graph/-graph/index.md).

### Types

| Name | Summary |
|---|---|
| [Format](-format/index.md) | `enum class Format` |

### Properties

| Name | Summary |
|---|---|
| [edges](edges.md) | `val edges: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>` |
| [format](format.md) | `val format: Format` |
| [triples](triples.md) | `val triples: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<`[`Triple`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-triple/index.html)`<`[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`>>` |
| [vertices](vertices.md) | `val vertices: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`>` |

### Companion Object Functions

| Name | Summary |
|---|---|
| [read](read.md) | Reads the GraphStore`fun read(vertx: Vertx, format: Format, dir: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): Future<`[`GraphStore`](./index.md)`>` |
| [write](write.md) | Writes the provided graph to the graph store`fun write(vertx: Vertx, format: Format, dir: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, graph: `[`Graph`](../../io.anima.graph/-graph/index.md)`): Future<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>` |
