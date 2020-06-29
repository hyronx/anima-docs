---
id: components
title: Chapter 2: Components
---

## The Basics

Basically the network only builds upon the database units which are the Minds and the managing and
communication units called Hives. The following illustration shows the interaction between those.

![Anima simple network](/img/anima_net_overview.png)
_Two Hives with three Minds each connected to each other_

### Mind

A Mind consists of the following parts:
* [A graph database](#graph-database)
* [An event bus](#event-bus)
* [A web interface](#web-interface)
* [An extensible data transformation system](#transformation-system)
* [Zero or more Nerves doing heavy processing](#nerves)

It stores a subset of the whole knowledge in the network.
As a provider you can control what kind of information you want to store
and optionally extend.

#### Graph database

The database must be Gremlin-enabled and can either be
the embedded Tinkerpop implementation or
an external DBMS like [JanusGraph](https://janusgraph.org/) or
the [Tinkerpop Gremlin Server](http://tinkerpop.apache.org/). This is the place
where data is permanently stored. Think of it like the long-term memory.

#### Event bus

The event bus is responsible for the communication between the different components.
Mainly it delivers status events and configuration changes across the system,
but also questions and their answers to the responsible processors and
may be extended with custom JSON-based events.
You can compare it to a nervous system between the body parts.

#### Web interface

The web interface consists a REST API for local administrative operations like
importing data or changing the configuration programmatically.
There is also WebSocket connection point which allows interaction with
the event bus. Both interfaces require the correct set of rights
at the local Mind. This could be compared to the senses like
vision, taste or listening which provide information to your brain about your environment.

#### Transformation system

The data transformation system is used internally for the conversion of
imported data to the final Gremlin graph.
Here any kind of conversion or enrichment of data is plausible.
A transformation is just function in mathematical terms and
responsible for converting data of type _A_ to data of type _B_.
To make another transformation available it must simply be registered
in the system and will than be called whenever data of type _A_ is requested
to be converted to type _B_.
More about the Transformation System can be found [here](/trafo).
Sadly a comparison to our body might not be feasible.
We can't just append a third arm and it just works _(tm)_.

#### Nerves

For more resource and time intensive work with the graph like reasoning or
natural language processing, involved components should not directly be loaded
into a Mind but be outsourced in a separate agent we call Nerve.
A Nerve communicates with its Mind through the already
described [WebSocket interface](#web-interface).

### Hive

Hives manage a set of Minds and connect with other Hives.
Basically they just forward requests they receive to all relevant connected systems.
They also cache answers and their requests
if the connected Minds didn't update their data.
