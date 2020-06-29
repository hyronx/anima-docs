[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](index.md) / [invoke](./invoke.md)

# invoke

`open fun invoke(inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>, context: `[`TransformationContext`](../-transformation-context/index.md)`): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Calls [transform](transform.md) on an input set.

You can override this method to control the returned set but
this shouldn't be necessary in most cases. Remember:
[invoke](./invoke.md) is expected to be pure.

### Parameters

`inputs` - The input set

`context` - The transformation context for this execution

**Return**
A future containing the result set

`open operator fun invoke(vararg inputs: A, context: `[`TransformationContext`](../-transformation-context/index.md)`? = null): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Call [transform](transform.md) on an input set.

Calls the [transform](transform.md) methods and is just a nicety.

### Parameters

`inputs` - The input set

**Return**
A future containing the result set

`operator fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> invoke(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Builds a transformation tree to transform the inputs to a set of outputs.

This method is the gate to all registered transformations. Out of them
it builds a transformation tree which is capable of transform some input to
the expected output based on their types. The output of all leaves of the tree
is merged into one set. How to work the resulting set is up to you.

### Parameters

`inputType` - The input type

`outputType` - The output type

`inputs` - Set of one or more inputs

### Exceptions

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](invoke.md#A) to [B](invoke.md#B).

**Return**
A future containing the set of results

`operator fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> invoke(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Builds a transformation tree to transform the inputs to a set of outputs.

This method is the gate to all registered transformations. Out of them
it builds a transformation tree which is capable of transform some input to
the expected output based on their types. The output of all leaves of the tree
is merged into one set. How to work the resulting set is up to you.

### Parameters

`inputType` - The input type

`outputType` - The output type

`inputs` - One or more inputs which represent an input set

### Exceptions

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](invoke.md#A) to [B](invoke.md#B).

**Return**
A future containing the set of results

`operator fun <reified A : `[`Immutable`](../-immutable/index.md)`, reified B : `[`Immutable`](../-immutable/index.md)`> invoke(vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Builds a transformation tree to transform the inputs to a set of outputs.

This method is the gate to all registered transformations. Out of them
it builds a transformation tree which is capable of transform some input to
the expected output based on their types. The output of all leaves of the tree
is merged into one set. How to work the resulting set is up to you.

### Parameters

`inputs` - One or more inputs which represent an input set

### Exceptions

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](invoke.md#A) to [B](invoke.md#B).

**Return**
A future containing the set of results

