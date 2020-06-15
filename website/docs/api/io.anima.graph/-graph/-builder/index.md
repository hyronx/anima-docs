[anima](../../../index.md) / [io.anima.graph](../../index.md) / [Graph](../index.md) / [Builder](./index.md)

# Builder

`class Builder`

### Types

| Name | Summary |
|---|---|
| [VertexWithEdge](-vertex-with-edge/index.md) | `data class VertexWithEdge<S : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, R : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`>` |

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `Builder()` |

### Functions

| Name | Summary |
|---|---|
| [build](build.md) | `fun build(): `[`Graph`](../index.md) |
| [meta](meta.md) | `fun meta(metaBuilder: Builder.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [relatedBy](related-by.md) | `infix fun <S : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, R : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`> S.relatedBy(edge: R): VertexWithEdge<S, R>` |
| [to](to.md) | `infix fun <S : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, R : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`, U : `[`Serializable`](https://docs.oracle.com/javase/6/docs/api/java/io/Serializable.html)`> VertexWithEdge<S, R>.to(vertex: U): S` |
