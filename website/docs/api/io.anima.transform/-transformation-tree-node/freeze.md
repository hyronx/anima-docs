[anima](../../index.md) / [io.anima.transform](../index.md) / [TransformationTreeNode](index.md) / [freeze](./freeze.md)

# freeze

`fun freeze(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)

Recursively freezes the whole tree

This method sets each node to frozen which disables the ability
to add children to a tree node making it effectively immutable.

