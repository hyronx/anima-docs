---
id: components
title: Components
---

## Components

Basically the network only builds upon the database units which are the Minds and the managing and
communication units called Hives. The following illustration shows the interaction between those. 

TODO: Insert simple illustration

### Mind

A Mind consists of the following parts:
* A graph database
* An event bus 
* A web interface
* A extensible data transformation system

It stores a subset of the whole knowledge in the network. As a provider you can control what kind of 
information you want to store and optionally extend.

The database must be Gremlin-enabled and can either be the embedded Tinkerpop implementation or 
an external DBMS like [JanusGraph](https://janusgraph.org/) or 
the [Tinkerpop Gremlin Server](http://tinkerpop.apache.org/). This is the place 
where data is permanently stored. Think of it like the long-term memory.

The event bus is responsible for the communication between the different components. Mainly it delivers
status events and configuration changes across the system. You can compare it to a nervous system between
the body parts.

The web interface consists a REST API for local administrative operations like importing data or changing
the configuration programmatically. There is also WebSocket connection point which allows interaction
with the event bus. Both interfaces require the correct set of rights at the local Mind. This could be
compared to the senses like vision, taste or listening which provide information to your brain.

The data transformation system is used for the conversion of imported data to the final Gremlin graph.
Here any kind of conversion or enrichment of data is plausible. A transformation is just function in 
mathematical terms and responsible for converting data of type A to data of type B. 
To make another transformation available it must simply be registered in the system and will than be
called whenever data of type A is requested to be converted to type B. Sadly a comparision to our body
might not be feasible. We can't just append a third arm and it just works _(tm)_.

### Hive

Hives manage a set of Minds and connect with other Hives. Basically they just forward any request 
they receive to all connected systems.

