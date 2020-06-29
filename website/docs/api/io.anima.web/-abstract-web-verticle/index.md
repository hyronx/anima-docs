[anima](../../index.md) / [io.anima.web](../index.md) / [AbstractWebVerticle](./index.md)

# AbstractWebVerticle

`abstract class AbstractWebVerticle : `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `AbstractWebVerticle()` |

### Properties

| Name | Summary |
|---|---|
| [bridgeOptions](bridge-options.md) | `open val bridgeOptions: BridgeOptions` |
| [providedServices](provided-services.md) | The provided services by this verticle`open val providedServices: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<Http>` |
| [sockJsOptions](sock-js-options.md) | `open val sockJsOptions: SockJSHandlerOptions` |

### Functions

| Name | Summary |
|---|---|
| [addHealthCheckRoute](add-health-check-route.md) | `fun Router.addHealthCheckRoute(): Route` |
| [processConfig](process-config.md) | Processes and customizes the full top level configuration object for the [start](../../io.anima/-anima-verticle/start.md) method.`open fun processConfig(fullConfig: JsonObject): JsonObject` |
| [setupRouter](setup-router.md) | `abstract fun setupRouter(config: `[`WebConfig`](../../io.anima.config/-web-config/index.md)`): Future<Router>` |
| [start](start.md) | Configures and sets up this verticle.`open fun start(startPromise: Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>, currentConfig: JsonObject): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [with](../../io.anima/with.md) | `infix fun `[`AnimaVerticle`](../../io.anima/-anima-verticle/index.md)`.with(state: `[`VerticleState`](../../io.anima/-verticle-state/index.md)`): `[`VerticleWithState`](../../io.anima/-verticle-with-state/index.md) |
