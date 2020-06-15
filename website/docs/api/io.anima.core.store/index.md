[anima](../index.md) / [io.anima.core.store](./index.md)

## Package io.anima.core.store

### Types

| Name | Summary |
|---|---|
| [GraphStore](-graph-store/index.md) | A graph representation divided in vertices, edges and triples`class GraphStore` |
| [GraphStoreReadTransformation](-graph-store-read-transformation/index.md) | Reads the graph store with the defined [storeFormat](#)`class GraphStoreReadTransformation : `[`Transformation`](../io.anima.transform/-transformation/index.md)`<`[`GraphStoreRead`](../io.anima.core.transform/-graph-store-read.md)`, `[`GraphStoreCapsule`](../io.anima.core.transform/-graph-store-capsule/index.md)`>` |
| [GraphStoreTransformation](-graph-store-transformation/index.md) | Transforms a graph store to a general Anima graph.`class GraphStoreTransformation : `[`Transformation`](../io.anima.transform/-transformation/index.md)`<`[`GraphStoreCapsule`](../io.anima.core.transform/-graph-store-capsule/index.md)`, `[`AnimaGraphCapsule`](../io.anima.transform/-anima-graph-capsule/index.md)`>` |
| [GraphStoreVerticle](-graph-store-verticle/index.md) | `class GraphStoreVerticle : `[`AnimaVerticle`](../io.anima/-anima-verticle/index.md) |
| [GraphStoreWriteTransformation](-graph-store-write-transformation/index.md) | Writes an [AnimaGraphCapsule](../io.anima.transform/-anima-graph-capsule/index.md) to the graph store with the defined [storeFormat](#)`class GraphStoreWriteTransformation : `[`SideEffect`](../io.anima.transform/-side-effect/index.md)`<`[`AnimaGraphCapsule`](../io.anima.transform/-anima-graph-capsule/index.md)`>` |
