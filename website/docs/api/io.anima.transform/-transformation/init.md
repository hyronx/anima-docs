[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](index.md) / [init](./init.md)

# init

`fun init(vertx: Vertx): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Initialises [vertx](init.md#io.anima.transform.Transformation.Companion$init(io.vertx.core.Vertx)/vertx).

It must be call early during application initialisation. Otherwise
[publishStatus](publish-status.md) won't work and throw [IllegalStateException](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-illegal-state-exception/index.html).

