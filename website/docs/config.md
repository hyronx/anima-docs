---
id: config
title: Configuration
---

The configuration in Anima relies on one YAML file, usually to be found
in the directory `conf`. As Minds and Hives are constructed of modules,
these modules may sometimes require additional configuration files.
To get information about them, please consult their specific documentation

## The Anima configuration file v1

The following YAML specification gives typed information about each entry.
You will encounter properties which may be `null` and can also be omitted.

```yaml
version: string # The version of this configuration file according to this specification
name: string # The name of this node
host: string # The public DNS name of this node
env: "test"|"production" # The environment of this node
passive: boolean # Decides whether to automatically connect to Hives or not
hives: # Array of Hive connection information
  - host: string # The public DNS name of a Hive
    port: integer # The port of that Hive
    username: string|null # An optional username if required by that Hive
    password: string|null # An optional password if required by that Hive
modules: # Array of module configurations
  - provider: string # The name in canonical form of a class which loads the module
    name: string|null # The name of that module as referenced by logs etc.
    config: object|null # A custom configuration object as required by that module
```

This is the general configuration file you will always find. The next parts
describe configurations for different modules.

## Modules

Module configurations must always be placed as already discussed above
under the `modules` key. Ensure that their classes are correctly loaded.
Otherwise the startup process will fail unrecoverably.

Because of currently fast development and change cycles, this documentations
might soon be out of date. As a first aid, check the Kotlin classes in the `config`
package of the problematic module to find the current configuration definition
if this one isn't up-to-date anymore.

### Mind

Provides a web interface for Minds and provides graph related data storage
and management classes.

```yaml
  - provider: io.anima.mind.MindVerticle # This is the loading class
    name: mind # This is a common name for this module
    config:
      data:
        tags: Array<string> # Defines tags to be accepted and requested by this Mind
      web:
        port: integer # [10180] Defines the port at which the web interface will listen
        api: # Defines API routes for the web interface
        # The following one is an example for the Import route.
        # They always have a name and contain custom properties
          - name: import
            acceptedTypes:
              application/rdf+xml: "io.anima.owl.RdfXmlInput"
              text/turtle: "io.anima.owl.RdfTurtleInput"
        frontend: # Defines the frontend configuration
          path: string # Where to find the frontend files
          allowRootFsAccess: boolean # Whether to allow full filesystem access
```

### Hive

Provides a web interface for connecting parties like Minds, other Hives or
clients like the frontend. It also handles event forwarding.

```yaml
  - provider: io.anima.hive.HiveVerticle
    name: hive
    config:
      web:
        port: string # [10180] Same as Mind
```

### Rules

Loads rules which process incoming data.

```yaml
  - provider: io.anima.RulesVerticle
    name: rules
    config:
      rules: Array<string> # Defines a set of Rule classes in canonical form to be loaded
```

### Question to transformation

Provides a gateway for questions and their answers
to be processed by the transformation system.
This is part of the `core`.

```yaml
  - provider: io.anima.mind.QuestionToTransformationVerticle
    name: questionToTrafo
```

### OWL

Provides classes for processing and importing of RDF, RDFS or OWL graphs.

```yaml
  - provider: io.anima.owl.OwlMainVerticle
    name: owl
```

### draw.io

Provides classes for process and importing of draw.io/diagrams.net diagrams
as graphs. They must have a special form which will soon be documented here.

```yaml
  - provider: "io.anima.DrawIoMainVerticle"
    name: drawio
```

### Internal memory cache

Loads the default cache implementation.
This is part of the `core`.

```yaml
  - provider: io.anima.core.cache.MemoryCacheVerticle
    name: cache
```

### Graph store

Loads the default graph store implementation. Currently only JSON is supported
as a format. You don't need to load this module if you use an external
Gremlin database.

```yaml
  - provider: io.anima.store.GraphStoreVerticle
    name: graphStore
    config:
      directory: string # [data]
      format: json
      maxSize: string # [1GB] The maximum size of the store with a unit
```
