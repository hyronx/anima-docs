[anima](../../../index.md) / [io.anima.graph](../../index.md) / [Graph](../index.md) / [Builder](./index.md)

# Builder

`class Builder`

### Types

| Name | Summary |
|---|---|
| [Triple](-triple/index.md) | `data class Triple<LV : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, E : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, RV : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`>` |
| [VertexWithEdge](-vertex-with-edge/index.md) | `data class VertexWithEdge<S : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, R : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`>` |

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `Builder()` |

### Functions

| Name | Summary |
|---|---|
| [at](at.md) | `infix fun <S : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, R : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, U : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`> Triple<S, R, U>.at(layer: `[`Layer`](../../-layer/index.md)`): S` |
| [build](build.md) | `fun build(): `[`Graph`](../index.md) |
| [relatedBy](related-by.md) | `infix fun <S : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, R : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`> S.relatedBy(edge: R): VertexWithEdge<S, R>` |
| [to](to.md) | `infix fun <S : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, R : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, U : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`> VertexWithEdge<S, R>.to(vertex: U): Triple<S, R, U>` |
