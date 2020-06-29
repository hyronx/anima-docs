[anima](../index.md) / [io.anima.transform](index.md) / [sideEffect](./side-effect.md)

# sideEffect

`fun <A : `[`Immutable`](-immutable/index.md)`> sideEffect(transformationName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, consumeHandler: (A, Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`SideEffect`](-side-effect/index.md)`<A>`

Creates a new side effect transformation.

You can use this method to create simple side effect handlers.

### Parameters

`transformationName` - The name for the transformation as seen in logs

`inputType` - The input type

`consumeHandler` - The handler consuming the input

**See Also**

[buildTransformation](build-transformation.md)

**Return**
A new SideEffect for input type [A](side-effect.md#A)

`inline fun <reified A : `[`Immutable`](-immutable/index.md)`> sideEffect(transformationName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, noinline consumeHandler: (A, Promise<`[`Void`](https://docs.oracle.com/javase/6/docs/api/java/lang/Void.html)`>) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`SideEffect`](-side-effect/index.md)`<A>`

Creates a new side effect transformation.

You can use this method to create simple side effect handlers.
This is the inline reified version of [sideEffect](./side-effect.md).

### Parameters

`transformationName` - The name for the transformation as seen in logs

`consumeHandler` - The handler consuming the input

**See Also**

[buildTransformation](build-transformation.md)

**Return**
A new SideEffect for input type [A](side-effect.md#A)

