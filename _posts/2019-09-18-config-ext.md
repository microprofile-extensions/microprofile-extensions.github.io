---
layout: default
title:  "Config Extensions"
date:   2016-07-16 12:00:00 -0400
categories: config
---

# Config sources and converters

Here you will find a collection of MicroProfile Config Extensions

[Github project page](https://github.com/microprofile-extensions/config-ext)

## Config sources

The following config sources is currently available:

* Memory config source
* File config source
* Etcd config source

### Memory config source

This allows you to create and override config value in memory via REST

```xml
    <dependency>
        <groupId>org.microprofile-ext.config-ext</groupId>
        <artifactId>configsource-memory</artifactId>
        <version>XXX</version>
    </dependency>
```

You can then change the value of a config:

    curl -X PUT "http://localhost:7080/profiling/api/microprofile-ext/memoryconfigsource/key/some.key" -H  "accept: */*" -H  "Content-Type: text/plain" -d "some.value"

And get the value of a config:

    curl -X GET "http://localhost:7080/profiling/api/microprofile-ext/memoryconfigsource/key/some.key" -H  "accept: */*"

### File config source

@TODO

### Etcd config source

@TODO

## Config converters

The following config converters is currently available:

* List config converter (List and Array)
* Json config converter (JsonObject and JsonArray)

### List and Array converter

@TODO

### JsonObject and JsonArray converters

@TODO

