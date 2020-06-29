[anima](../../index.md) / [io.anima.transform](../index.md) / [SideEffect](index.md) / [invoke](./invoke.md)

# invoke

`operator fun <A : `[`Immutable`](../-immutable/index.md)`> invoke(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<NoResult>>`

Builds a transformation tree to execute a set of side effects.

### Parameters

`inputType` - The input type

`inputs` - Set of one or more inputs

### Exceptions

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](invoke.md#A) to [B](#).

**See Also**

[Transformation.invoke](../-transformation/invoke.md)

**Return**
A future containing the set of results

`operator fun <A : `[`Immutable`](../-immutable/index.md)`> invoke(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<NoResult>>`

Builds a transformation tree to execute a set of side effects.

### Parameters

`inputType` - The input type

`inputs` - One or more inputs which represent an input set

### Exceptions

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](invoke.md#A) to [B](#).

**See Also**

[Transformation.invoke](../-transformation/invoke.md)

**Return**
A future containing the set of results

`operator fun <reified A : `[`Immutable`](../-immutable/index.md)`> invoke(vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<NoResult>>`

Builds a transformation tree to execute a set of side effects.

### Parameters

`inputs` - One or more inputs which represent an input set

### Exceptions

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](invoke.md#A) to [B](#).

**Return**
A future containing the set of results

