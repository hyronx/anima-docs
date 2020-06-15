[anima](../../index.md) / [io.anima](../index.md) / [AnimaVerticle](index.md) / [handleDeploymentResult](./handle-deployment-result.md)

# handleDeploymentResult

`protected open fun <A : `[`AnimaVerticle`](index.md)`> handleDeploymentResult(childClass: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, promise: Promise<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>): (AsyncResult<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)
`protected fun <reified A : `[`AnimaVerticle`](index.md)`> handleDeploymentResult(promise: Promise<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>): (AsyncResult<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Returns a handler for the deployment result of a child verticle.

