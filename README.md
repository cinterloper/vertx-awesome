# Awesome Vert.x [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

*Awesome Vert.x* is a list of awesome frameworks, libraries or other components for use with or that use
[Vert.x](https://github.com/eclipse/vert.x) version 3.

If you want your component to appear here send a pull request to this repository to add it.

Please note that we can't vouch for the stability or production-worthiness of everything on this list unless it has
the icon ![(stack)](stack.png "Vert.x Stack") next to it. This icon means the component
is part of the official [Vert.x stack](http://vert-x3.github.io/docs/).

For Vert.x version 2 check [this page](./vert-x2.md).

## Contents

- [Web Frameworks](#web-frameworks)
- [Authentication Authorisation](#authentication-authorisation)
- [Database Clients](#database-clients)
- [Integration](#integration)
- [Middleware](#middleware)
- [Language Support](#language-support)
- [Reactive](#reactive)
- [Sync Thread Non Block](#sync-thread-non-block)
- [Vert.x Event Bus Clients](#vertx-event-bus-clients)
- [Cluster Managers](#cluster-managers)
- [Cloud Support](#cloud-support)
- [Docker](#docker)
- [Search Engines](#search-engines)
- [Service Factory](#service-factory)
- [Dependency Injection](#dependency-injection)
- [Testing](#testing)
- [Development Tools](#development-tools)
- [Miscellaneous](#miscellaneous)
- [Distribution](#distribution)
- [Examples](#examples)
- [Deployment](#deployment)
- [Utilities](#utilities)

## Web Frameworks

* [Vert.x Web](https://github.com/vert-x3/vertx-web)  ![(stack)](stack.png "Vert.x Stack") - Full featured web toolkit for Vert.x.
* [Vert.x Jersey](https://github.com/englishtown/vertx-jersey) - Create JAX-RS [Jersey](https://jersey.java.net/) resources in Vert.x.
* [Vert.x Nubes](https://github.com/aesteve/vertx-nubes) - Provides an annotation layer on top of Vert.x Web.
* [Kovert](https://github.com/kohesive/kovert) - Invisible REST framework for Kotlin + Vert.x Web.
* [RestVertx](https://github.com/codesipcoffee/restvertx) - Easily build HTTP services in Vert.x using Java.
* [Handlers](https://github.com/spriet2000/vertx-handlers-http) - Open web framework for Vert.x.
* [QBit](https://github.com/advantageous/qbit) - REST and WebSocket method call marshaling and reactive library.
* [vertx-rest-storage](https://github.com/swisspush/vertx-rest-storage) - Persistence for REST resources in the filesystem or a redis database.
* [Jubilee](https://github.com/isaiah/jubilee) - A rack compatible Ruby HTTP server built on Vert.x 3.
* [katharsis-vertx](https://github.com/katharsis-project/katharsis-vertx) - [JSONAPI](http://jsonapi.org/) implementation for Vert.x 3.

## Authentication Authorisation

* [Vert.x Auth JDBC](https://github.com/vert-x3/vertx-auth/tree/master/vertx-auth-jdbc)  ![(stack)](stack.png "Vert.x Stack") - Vert.x authentication/authorisation JDBC based.
* [Vert.x Auth JWT](https://github.com/vert-x3/vertx-auth/tree/master/vertx-auth-jwt)  ![(stack)](stack.png "Vert.x Stack") - Vert.x Authorisation based on JSON Web Tokens.
* [Vert.x Auth Shiro](https://github.com/vert-x3/vertx-auth/tree/master/vertx-auth-shiro)  ![(stack)](stack.png "Vert.x Stack") - Vert.x AuthN/AuthZ based on [Apache Shiro](http://shiro.apache.org/).
* [Vert.x-Pac4j](https://github.com/pac4j/vertx-pac4j)    ![(stack)](stack.png "Vert.x Stack") - Vert.x authentication/authorisation implemented using [pac4j](http://www.pac4j.org/).

## Database Clients

*Clients for connecting to databases*

* Relational Databases
  * [JDBC](https://github.com/vert-x3/vertx-jdbc-client) ![(stack)](stack.png "Vert.x Stack") - Asynchronous interface around a JDBC datasource.
  * [MySQL](https://github.com/vert-x3/vertx-mysql-postgresql-client) - Asynchronous client for MySQL.
  * [PostgreSQL](https://github.com/vert-x3/vertx-mysql-postgresql-client) - Asynchronous client for PostgreSQL.
  * [database](https://github.com/susom/database) - Client for Oracle, PostgreSQL, SQL Server, HyperSQL, etc. designed for security, correctness, and ease of use.

* NoSQL Databases
  * [MongoDB](https://github.com/vert-x3/vertx-mongo-client) ![(stack)](stack.png "Vert.x Stack") - An asynchronous client for interacting with a MongoDB database.
  * [Redis](https://github.com/vert-x3/vertx-redis-client) ![(stack)](stack.png "Vert.x Stack") - Asynchronous API to interact with Redis.
  * [Cassandra](https://github.com/englishtown/vertx-cassandra) - Asynchronous API to interact with Cassandra and Cassandra Mapping.
  * [OrientDB](https://github.com/cstamas/vertx-orientdb) - Non-blocking OrientDB server integration.

* [vertx-pojo-mapper](https://github.com/BraintagsGmbH/vertx-pojo-mapper) - Non-blocking POJO mapping for MySQL and MongoDB.


## Integration

* Server-Sent Events
  * [jEaSSE](https://github.com/mariomac/jeasse) - Java Easy SSE. A simple, lightweight implementation of SSE.

* Mail
  * [SMTP](https://github.com/vert-x3/vertx-mail-client) ![(stack)](stack.png "Vert.x Stack") - Async SMTP client.
  * [vertx-smtp-server] (https://github.com/cinterloper/vertx-smtp-server) - SMTP server bridging to EventBus.

* REST
  * [Vertx REST Client](https://github.com/hubrick/vertx-rest-client) - A REST client for vertx with support for RxJava and request caching.

* Messaging
  * [AMQP 1.0](https://github.com/vert-x3/vertx-amqp-bridge) ![(stack)](stack.png "Vert.x Stack") - Interact with AMQP 1.0 servers using the Vert.x Producer and Consumer APIs.
  * [RabbitMQ](https://github.com/vert-x3/vertx-rabbitmq-client) ![(stack)](stack.png "Vert.x Stack") - A RabbitMQ client (AMQP 0.9.1).
  * [kafka](https://github.com/cyngn/vertx-kafka) - Kafka client for consuming and producing messages.
  * [Kafka Service](https://github.com/hubrick/vertx-kafka-service) - Kafka producer and consumer with retry logic.
  * [SaltStack] (https://github.com/cinterloper/vertx-salt) - A bi-directional bridge between the SaltStack event system and the Vert.x event bus.
  * [ZeroMQ](https://github.com/dano/vertx-zeromq) - ZeroMQ Event Bus bridge.
  * [MQTT Broker](https://github.com/GruppoFilippetti/vertx-mqtt-broker) - MQTT Broker (MQTT ver. 3.1.1 and 3.1 compliant).
  * [Azure ServiceBus](https://github.com/TextBack/vertx-azure-servicebus) - Azure [ServiceBus](https://azure.microsoft.com/en-us/services/service-bus/) producer and consumer (fully async, doesn't use Microsoft Azure SDK).
  
* JavaEE
  * [JCA adaptor](https://github.com/vert-x3/vertx-jca) ![(stack)](stack.png "Vert.x Stack") - Java Connector Architecture Adaptor for the Vert.x event bus.
  * [Weld](https://github.com/weld/weld-vertx) - Brings the CDI programming model into the Vert.x ecosystem (register CDI observer methods as Vert.x message consumers, CDI-powered Verticles, define routes in a declarative way, etc.).

* Meteor
  * [Meteor](https://github.com/jmusacchio/vertxbus/) - Meteor integration support through Vert.x event bus.

* Metrics
  * [Hawkular metrics](https://github.com/tsegismont/vertx-monitor) - [Hawkular](http://www.hawkular.org/) implementation of the Vert.x Metrics SPI.
  * [DropWizard metrics](https://github.com/vert-x3/vertx-dropwizard-metrics) ![(stack)](stack.png "Vert.x Stack") - Metrics implementation using DropWizard metrics.
  * [OpenTsDb Metrics](https://github.com/cyngn/vertx-opentsdb) - [OpenTsDb](http://opentsdb.net/) metrics client for Vert.x.
  * [Bosun Monitoring](https://github.com/cyngn/vertx-bosun) - [Bosun](https://bosun.org/) client library for Vert.x.

* Netflix - Hystrix
  * [Hystrix Metrics Stream](https://github.com/kennedyoliveira/hystrix-vertx-metrics-stream.git) - Emits metrics for Hystrix Dashboard from a Vertx application with [Hystrix](https://github.com/Netflix/Hystrix).

## Middleware

* [Gateleen](https://github.com/swisspush/gateleen) - Middleware library based on Vert.x to build advanced JSON/REST communication servers

## Language Support

*Programming language support for Vert.x*

* [Ceylon](https://github.com/vert-x3/vertx-lang-ceylon) ![(stack)](stack.png "Vert.x Stack") - Ceylon support.
* [Groovy](https://github.com/vert-x3/vertx-lang-groovy) ![(stack)](stack.png "Vert.x Stack") - Groovy support.
* [Java](https://github.com/eclipse/vert.x) ![(stack)](stack.png "Vert.x Stack") - Vert.x main repository (including the Java API).
* [JavaScript](https://github.com/vert-x3/vertx-lang-js) ![(stack)](stack.png "Vert.x Stack") - JavaScript support.
* [Python](https://github.com/vert-x3/vertx-lang-python) - Python support.
* [Ruby](https://github.com/vert-x3/vertx-lang-ruby) ![(stack)](stack.png "Vert.x Stack") - Ruby support.
* [Scala](https://github.com/vert-x3/vertx-lang-scala) - Scala support.
* [TypeScript](https://github.com/michel-kraemer/vertx-lang-typescript) - TypeScript support.
* [Kotlin](https://github.com/cy6erGn0m/vertx3-lang-kotlin) - Kotlin support.

*Language extensions*

* [Grooveex](https://github.com/aesteve/grooveex) - Syntaxic sugar + utilities (DSL builders, etc.) on top of [vertx-lang-groovy](https://github.com/vert-x3/vertx-lang-groovy).

## Reactive

* [Reactive Streams](https://github.com/vert-x3/vertx-reactive-streams) ![(stack)](stack.png "Vert.x Stack") - Vert.x Reactive Streams.
* [Reactive Extensions](https://github.com/vert-x3/vertx-rx) ![(stack)](stack.png "Vert.x Stack") - Vert.x Reactive Extensions.
* [vertx-util](https://github.com/cyngn/vertx-util) - Light weight promises & latches for Vert.x.
* [QBit](https://github.com/advantageous/qbit) - Async typed actor-like lib that runs easily in Vert.x Async Callbacks. Callback management.

## Sync Thread Non Block

* [Sync](https://github.com/vert-x3/vertx-sync) - Synchronous but non-OS-thread-blocking verticles.

## Vert.x Event Bus Clients

*Clients to connect applications to the Vert.x event bus*

* [JavaScript](https://www.npmjs.com/package/vertx3-eventbus-client) ![(stack)](stack.png "Vert.x Stack") - JavaScript event bus client.
* [C++11](https://github.com/julien3/vertxbuspp) - C++11 event bus client.
* [Java](https://github.com/saffron-technology/vertx-eventbusbridge) - Java implementation of vertxbus.js.
* [Java](https://github.com/abdlquadri/vertx-eventbus-java) - Java and Android Event Bus Client.
* [CLI](https://github.com/cinterloper/vxc) - Command-line binary client for Vert.x event bus - pipe in JSON, emit JSON.

## Cluster Managers

*Implementations of the Vert.x cluster manager SPI*

* [Hazelcast Cluster Manager](https://github.com/vert-x3/vertx-hazelcast) ![(stack)](stack.png "Vert.x Stack") - Hazelcast cluster manager.
* [Ignite Cluster Manager](https://github.com/vert-x3/vertx-ignite) ![(stack)](stack.png "Vert.x Stack") - Ignite cluster manager.
* [JGroups Cluster Manager](https://github.com/vert-x3/vertx-jgroups) - JGroups cluster manager.
* [Zookeeper Cluster Manager](https://github.com/stream1984/vertx-zookeeper) - Zookeeper cluster manager.
* [Atomix Cluster Manager](https://github.com/atomix/atomix-vertx) - An [Atomix](http://atomix.io) based cluster manager implementation for Vert.x 3.

## Cloud Support

* [OpenShift DIY cartridge](https://github.com/vert-x3/vertx-openshift-diy-quickstart) ![(stack)](stack.png "Vert.x Stack") - OpenShift DIY Cartridge using Vert.x.
* [OpenShift Vert.x cartridge](https://github.com/vert-x3/vertx-openshift-cartridge) ![(stack)](stack.png "Vert.x Stack") - OpenShift Vert.x Cartridge using Vert.x.

## Docker

* [Docker images](https://github.com/vert-x3/vertx-stack/tree/master/stack-docker) ![(stack)](stack.png "Vert.x Stack") - Docker images for Vert.x.

## Search Engines

* [Vert.x Elasticsearch Service](https://github.com/englishtown/vertx-elasticsearch-service) - Vert.x 3 [Elasticsearch](https://www.elastic.co/) service with event bus proxying.
* [Vert.x Solr Service](https://github.com/englishtown/vertx-solr-service) - Vert.x 3 Solr service with event bus proxying.

## Service Factory

* [Service Factory](https://github.com/vert-x3/vertx-service-factory) ![(stack)](stack.png "Vert.x Stack") - Vert.x Service Factory.
* [Maven Service Factory](https://github.com/vert-x3/vertx-maven-service-factory) ![(stack)](stack.png "Vert.x Stack") - Maven Vert.x Service Factory.
* [HTTP Service Factory](https://github.com/vert-x3/vertx-http-service-factory) ![(stack)](stack.png "Vert.x Stack") - Vert.x HTTP Service Factory.
* [Node.js Service Factory](https://github.com/mellster2012/vertx-nodejs-service-factory) - Vert.x Node.js Service Factory.
* [Eclipse SISU Service Factories](https://github.com/cstamas/vertx-sisu) - Vert.x integration with [Eclipse SISU](https://www.eclipse.org/sisu/) DI container offering alternatives for `vertx-service-factory` and `vertx-maven-service-factory`.

## Dependency Injection

* [Vert.x Guice](https://github.com/englishtown/vertx-guice) - Vert.x verticle factory for Guice dependency injection.
* [Vert.x HK2](https://github.com/englishtown/vertx-hk2) - Vert.x verticle factory for HK2 dependency injection.
* [Spring Vert.x Extension](https://github.com/amoAHCP/spring-vertx-ext) - Vert.x verticle factory for Spring DI injection.
* [Vert.x Beans](https://github.com/rworsnop/vertx-beans) - Inject Vert.x objects as beans into your Spring application.
* [QBit](https://github.com/advantageous/qbit) - QBit works with Spring DI and Spring Boot (and of course Vertx). Allows you to use QBit, Vertx, Spring DI and Spring Boot in the same application.
* [Vert.x Eclipse SISU](https://github.com/cstamas/vertx-sisu) - Vert.x integration with [Eclipse SISU](https://www.eclipse.org/sisu/) DI container.

## Testing

* [Vert.x Unit](https://github.com/vert-x3/vertx-unit) ![(stack)](stack.png "Vert.x Stack") - Async polyglot unit testing for Vert.x.

## Development Tools

* [Vert.x Hot](https://github.com/dazraf/vertx-hot) - A Maven plugin for the hot-deploy of Maven Vert.x projects.

## Miscellaneous

* [Vert.x Child Process](https://github.com/vietj/vertx-childprocess) - Spawn child process from Vert.x.
* [vertx-redisques](https://github.com/swisspush/vertx-redisques) - A highly scalable redis-persistent queuing system for Vert.x.

## Distribution

* [Vert.x Stack](https://github.com/vert-x3/vertx-stack) ![(stack)](stack.png "Vert.x Stack") - Vert.x + the endorsed modules.

## Examples

* [Vert.x examples](https://github.com/vert-x3/vertx-examples) ![(stack)](stack.png "Vert.x Stack") - The official Vert.x examples including web examples, how to use the official database clients, etc.
* [Vert.x feeds](https://github.com/aesteve/vertx-feeds) - Example of an RSS aggregator built using Vert.x, Gradle, MongoDB, Redis, Handlebars templates, AngularJS, the event bus and SockJS.
* [Vert.x Markdown service](https://github.com/aesteve/vertx-markdown-service) - Example on how to use [service-proxy](https://github.com/vert-x3/vertx-service-proxy) with Gradle.
* [Example using event bus and service proxies to connect vertx and node](https://github.com/advantageous/vertx-node-ec2-eventbus-example) - Step by step example with wiki description showing how to connect Vert.x and Node using event bus and service proxies.

## Deployment

* [Vert.x Deploy Application](https://github.com/msoute/vertx-deploy-tools) - (Seamless) deploy to AWS based Vert.x application clusters.

## Utilities

* [Chime](https://github.com/LisiLisenok/Chime) - Time scheduler working on Vert.x event bus allowing for scheduling with _cron-style_ and _interval_ timers.
* [Vert.x Cron](https://github.com/diabolicallabs/vertx-cron) - Schedule events with cron specifications. Has event bus and Observable versions.
* [Vert.x POJO config](https://github.com/aesteve/vertx-pojo-config) - Allows for mapping between standard JSON configuration and a (type-safe) configuration Java bean. Also allows the configuration bean to be validated through JSR 303.
