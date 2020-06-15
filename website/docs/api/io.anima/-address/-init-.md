[anima](../../index.md) / [io.anima](../index.md) / [Address](index.md) / [&lt;init&gt;](./-init-.md)

# &lt;init&gt;

`Address(namespace: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`)`

Defines a event address

This address also is a [AnimaRessourceIdentifier](../-anima-ressource-identifier/index.md) (short ARI).
As that its format is as follows:
`anima:Address:<app>:<path>`
`<app>` should be replaced by a application or package name in reverse domain name form.
`<path>` is slash (`/`) separated path which has no special meaning.

An example of such ARI would be:
`anima:Address:io.anima.core:/config/update`
You should be able to confirm that with the following piece of code:
`println(Address.ConfigUpdate.toARI())`

[io.vertx.core.eventbus.MessageConsumer](#)s should listen to the full ARI.

