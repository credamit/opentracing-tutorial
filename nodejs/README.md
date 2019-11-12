# OpenTracing Tutorial - Node.js

## Installing

The tutorials are using CNCF Jaeger (https://github.com/jaegertracing/jaeger) as the tracing backend,
[see here](../README.md) how to install it in a Docker image.

First clone the [opentracing-tutorial](https://github.com/yurishkuro/opentracing-tutorial), then install the dependencies:

```
cd opentracing-tutorial/nodejs
npm install
```

The rest of the commands in the Node.js tutorials should be executed relative to this `nodejs` directory.


## Lessons

* [Lesson 01 - Hello World](./lesson01)
  * Instantiate a Tracer
  * Create a simple trace
  * Annotate the trace
* [Lesson 02 - Context and Tracing Functions](./lesson02)
  * Trace individual functions
  * Combine multiple spans into a single trace
  * Propagate the in-process context
* [Lesson 03 - Tracing RPC Requests](./lesson03)
  * Trace a transaction across more than one microservice
  * Pass the context between processes using `Inject` and `Extract`
  * Apply OpenTracing-recommended tags
* [Lesson 04 - Baggage](./lesson04)
  * Understand distributed context propagation
  * Use baggage to pass data through the call graph
* [Extra Credit](./extracredit)
  * Use existing open source instrumentation
