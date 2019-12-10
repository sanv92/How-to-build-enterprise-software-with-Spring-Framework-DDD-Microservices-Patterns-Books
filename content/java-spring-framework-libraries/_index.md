+++
title = "Java / Spring Framework Libraries"
description = "Java / Spring Framework Libraries"
chapter = true
weight = 1
pre = "<b>1. </b>"
+++

# Java / Spring Framework Libraries
---

#### CQRS (command-query responsibility segregation) + EVENT SOURCING
- https://axoniq.io/ - framework and server for event-driven microservices

<hr />

#### Test-driven development (TDD)
- https://testcontainers.org/ - java library that supports JUnit tests, providing lightweight, throwaway instances of common databases, Selenium web browsers, or anything else that can run in a Docker container.
    * fast to configure,
    * forget about environmental problems, when Selenium chrome driver updates,
    * no need configure, use docker containers,
    * ports are configured automatically,
    * you will trust your tests, because you run tests, with the same configuration and environments, as in production.
- https://junit.org/
- https://site.mockito.org/
- http://rest-assured.io/ - fluent HTTP end-to-end API testing, with BDD style (including given, when, then) to create code that is expressive as well as easy to read and understand,
is built on top of "**spring-mock-mvc**".

<hr />

#### Behavior-driven development (BDD)
- https://cucumber.io/

<hr />

#### Consumer-Driven Contracts (CDC)
- https://www.baeldung.com/spring-cloud-contract - consumer side integration tests for the API gateway use contracts to configure a dummy HTTP server simulating the behavior of the service (Install **spring-cloud-contract-wiremock** and **spring-cloud-contract-stub-runner** dependencies).
- http://wiremock.org/ - simulator for HTTP-based APIs. Some might consider it a service virtualization tool or a mock server,
use together with "**Spring Cloud Contract**".

<hr />

#### Message broker
- https://rabbitmq.com/
- https://kafka.apache.org/

<hr />

#### Central authentication & authorization
- https://keycloak.org/
- https://gluu.org/

<hr />

#### Logging
- http://www.slf4j.org/ - logging Facade for Java
- http://logback.qos.ch/ - logging frameworks (**use slf4j and logback together**)

##### **Elasticsearch Stack (the log aggregation infrastructure)**
The logging infrastructure is responsible for aggregating the logs, storing them, and enabling the user to search them. One popular logging infrastructure is the ELK stack. ELK consists of three open source products:

- https://www.elastic.co/products/elasticsearch Elasticsearch — A text search-oriented NoSQL database that’s used as the logging server.
- https://www.elastic.co/products/logstash Logstash — A log pipeline that aggregates the service logs and writes them to Elasticsearch.
- https://www.elastic.co/products/kibana Kibana — A visualization tool for Elasticsearch.

##### **AWS**
- https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html - AWS CloudWatch Log.

<hr />

#### Tracing system
- https://zipkin.io/

<hr />

#### Exception tracking services

- https://honeybadger.io/

#### In-Memory Computing Platform
- https://ignite.apache.org/
- https://hazelcast.com/

<hr />

#### Container Orchestration
- https://kubernetes.io/
- https://nomadproject.io/

<hr />

#### Container Network Manager (runtime diagnostics, metrics, logging, tracing, traffic security, traffic control)
- https://istio.io/
- https://linkerd.io/

<hr />

#### Api Gateway
- https://aws.amazon.com/api-gateway/ - create, maintain, and secure APIs at any scale
- https://netflix.github.io/falcor/starter/what-is-falcor.html - combine all rest-api data as a single Virtual JSON object

<hr />

#### Securely accessing secrets
- https://vaultproject.io/ - Hashicorp Vault

<hr />

#### Devops Tools
- https://www.ansible.com/
- https://terraform.io/
- https://jenkins.io/

<hr />

#### Other frameworks, similar as Spring Framework
- https://micronaut.io/
- https://quarkus.io/
- https://helidon.io/
