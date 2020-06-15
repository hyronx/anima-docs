[anima](../../index.md) / [io.anima.core](../index.md) / [HiveConnectionVerticle](./index.md)

# HiveConnectionVerticle

`class HiveConnectionVerticle : `[`BasicAnimaVerticle`](../../io.anima/-basic-anima-verticle/index.md)

Establishes and manages a connection to one Hive.

This verticle is created by [HiveClientVerticle](../-hive-client-verticle/index.md).
The connection is established following the SockJS protocol.
For further information reference the
[SockJS spec](http://sockjs.github.io/sockjs-protocol/sockjs-protocol-0.2.1.html).

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | Establishes and manages a connection to one Hive.`HiveConnectionVerticle()` |

### Functions

| Name | Summary |
|---|---|
| [start](start.md) | `fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
