[anima](../../index.md) / [io.anima.core.transform](../index.md) / [GremlinGraphSink](index.md) / [createAddressable](./create-addressable.md)

# createAddressable

`fun createAddressable(traversalSource: SparqlTraversalSource): `[`Transformation`](../../io.anima.transform/-transformation/index.md)`<`[`ExtendedAnimaGraphCapsule`](../../io.anima.transform/-extended-anima-graph-capsule/index.md)`, Explicit>`

Creates an instance of [GremlinGraphSink](index.md) as a transformation returning [Explicit](-explicit.md).

The returned transformation can explicitly be addressed by calling [Transformation.transform](../../io.anima.transform/-transformation/transform.md) with
the output type [Explicit](-explicit.md). Otherwise this instance won't be called.
Its [transform](../../io.anima.transform/-side-effect/transform.md) method will return an empty set.

### Parameters

`traversalSource` - A SPARQL-enabled [GraphTraversal](#)

**Return**
The new [GremlinGraphSink](index.md) object

