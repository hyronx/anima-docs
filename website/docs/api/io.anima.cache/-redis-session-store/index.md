[anima](../../index.md) / [io.anima.cache](../index.md) / [RedisSessionStore](./index.md)

# RedisSessionStore

`class RedisSessionStore : SessionStore`

### Functions

| Name | Summary |
|---|---|
| [clear](clear.md) | `fun clear(resultHandler: Handler<AsyncResult<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>>?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [close](close.md) | `fun close(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [createSession](create-session.md) | `fun createSession(timeout: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`): Session`<br>`fun createSession(timeout: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, length: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): Session` |
| [delete](delete.md) | `fun delete(id: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`?, resultHandler: Handler<AsyncResult<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>>?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [get](get.md) | `fun get(cookieValue: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`?, resultHandler: Handler<AsyncResult<Session>>?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [init](init.md) | `fun init(vertx: Vertx?, options: JsonObject?): SessionStore` |
| [put](put.md) | `fun put(session: Session?, resultHandler: Handler<AsyncResult<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>>?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [retryTimeout](retry-timeout.md) | `fun retryTimeout(): `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html) |
| [size](size.md) | `fun size(resultHandler: Handler<AsyncResult<`[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`>>?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
