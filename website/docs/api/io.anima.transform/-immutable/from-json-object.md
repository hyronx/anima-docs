[anima](../../index.md) / [io.anima.transform](../index.md) / [Immutable](index.md) / [fromJsonObject](./from-json-object.md)

# fromJsonObject

`fun <T : `[`Immutable`](index.md)`> fromJsonObject(json: JsonObject, type: `[`Class`](https://docs.oracle.com/javase/6/docs/api/java/lang/Class.html)`<T>): T!`

Converts [json](from-json-object.md#io.anima.transform.Immutable.Companion$fromJsonObject(io.vertx.core.json.JsonObject, java.lang.Class((io.anima.transform.Immutable.Companion.fromJsonObject.T)))/json) to an [Immutable](index.md) implementation as [type](from-json-object.md#io.anima.transform.Immutable.Companion$fromJsonObject(io.vertx.core.json.JsonObject, java.lang.Class((io.anima.transform.Immutable.Companion.fromJsonObject.T)))/type).

### Parameters

`json` - The [JsonObject](#) to be converted

`type` - The type to convert the JSON to

**Return**
The converted type

`fun <reified T : `[`Immutable`](index.md)`> fromJsonObject(json: JsonObject): T!`

Converts [json](from-json-object.md#io.anima.transform.Immutable.Companion$fromJsonObject(io.vertx.core.json.JsonObject)/json) to an [Immutable](index.md) implementation as type [T](from-json-object.md#T).

### Parameters

`json` - The [JsonObject](#) to be converted

**Return**
The converted type

