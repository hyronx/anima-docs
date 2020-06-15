[anima](../../index.md) / [io.anima.transform](../index.md) / [Transformation](index.md) / [invoke](./invoke.md)

# invoke

`open fun invoke(inputs: `[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<A>, context: `[`TransformationContext`](../-transformation-context/index.md)`): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Calls [transform](transform.md) on an input set.

You can override this method to control the returned set but
this shouldn't be necessary in most cases. Remember:
[transform](transform.md) is expected to be pure.

### Parameters

`inputs` - The input set

`context` - The transformation context for this execution

**Return**
A future containing the result set

`open operator fun invoke(vararg inputs: A, context: `[`TransformationContext`](../-transformation-context/index.md)`? = null): Future<`[`Set`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-set/index.html)`<B>>`

Call [transform](transform.md) on an input set.

Calls the [invoke](./invoke.md) methods and is just a nicety.

### Parameters

`inputs` - The input set

**Return**
A future containing the result set

