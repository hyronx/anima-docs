[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationBuilder](./index.md)

# TransformationBuilder

`class TransformationBuilder<A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`>`

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `TransformationBuilder(trafoName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, enableTimeout: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = true)` |

### Properties

| Name | Summary |
|---|---|
| [enableTimeout](enable-timeout.md) | `var enableTimeout: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [inputType](input-type.md) | `var inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>` |
| [outputType](output-type.md) | `var outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>` |

### Functions

| Name | Summary |
|---|---|
| [build](build.md) | Builds the actual [Transformation](../-transformation/index.md) object.`fun build(): `[`Transformation`](../-transformation/index.md)`<A, B>` |
| [filter](filter.md) | `fun filter(filterHandler: (input: A, context: `[`TransformationContext`](../-transformation-context/index.md)`) -> `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [invoke](invoke.md) | `fun invoke(invokeHandler: (inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>, context: `[`TransformationContext`](../-transformation-context/index.md)`) -> Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [transform](transform.md) | `fun transform(transformHandler: (input: A, outputPromise: Promise<B>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
