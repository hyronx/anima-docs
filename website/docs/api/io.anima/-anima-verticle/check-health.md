[anima](../../index.md) / [io.anima](../index.md) / [AnimaVerticle](index.md) / [checkHealth](./check-health.md)

# checkHealth

`open fun checkHealth(statusPromise: Promise<Status>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Returns health information for this verticle

Override this to customize the health status returned. This method is called if some frontend
requests information about the health status in the system or specifically this verticle.

### Parameters

`statusPromise` - A promise returning the status of this verticle