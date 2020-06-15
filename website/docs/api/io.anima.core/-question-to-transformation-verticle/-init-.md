[anima](../../index.md) / [io.anima.core](../index.md) / [QuestionToTransformationVerticle](index.md) / [&lt;init&gt;](./-init-.md)

# &lt;init&gt;

`QuestionToTransformationVerticle()`

Receives questions messages and transforms them to answers using the transformation system.

This class is a gateway for question messages to the transformation system.
In the future when the transformation system is directly address through [Address.TransformationRequested](../../io.anima/-address/-transformation-requested.md),
you won't need this class anymore. For this reason it must already be loaded as a module like this
in the config:

``` yaml
# config stuff before
modules:
  - provider: io.anima.core.QuestionToTransformationVerticle
    name: questionToTrafo
  # other modules
```

