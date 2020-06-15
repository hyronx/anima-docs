[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](index.md) / [transform](./transform.md)

# transform

`abstract fun transform(input: A, outputPromise: Promise<B>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Transforms the input to some output.

This method must be implemented as a pure function.

### Parameters

`input` - The input

`outputPromise` - A promise returning the output or an error

**Return**
Unit because the result is returned by [outputPromise](transform.md#io.anima.transform.Transformation$transform(io.anima.transform.Transformation.A, io.vertx.core.Promise((io.anima.transform.Transformation.B)))/outputPromise)

`open fun transform(input: A): Future<B!>`

Transforms the input to some output.

Implement the [transform](./transform.md) method.

### Parameters

`input` - The input

**Return**
A future returning the output or an error

`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> transform(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

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

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](transform.md#A) to [B](transform.md#B).

**Return**
A future containing the set of results

`fun <A : `[`Immutable`](../-immutable/index.md)`, B : `[`Immutable`](../-immutable/index.md)`> transform(inputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<A>, outputType: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<B>, vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

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

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](transform.md#A) to [B](transform.md#B).

**Return**
A future containing the set of results

`fun <reified A : `[`Immutable`](../-immutable/index.md)`, reified B : `[`Immutable`](../-immutable/index.md)`> transform(vararg inputs: A): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Builds a transformation tree to transform the inputs to a set of outputs.

This method is the gate to all registered transformations. Out of them
it builds a transformation tree which is capable of transform some input to
the expected output based on their types. The output of all leaves of the tree
is merged into one set. How to work the resulting set is up to you.

### Parameters

`inputs` - One or more inputs which represent an input set

### Exceptions

`NoPathsFoundException` - Thrown if there is no way with current transformations to transform [A](transform.md#A) to [B](transform.md#B).

**Return**
A future containing the set of results

