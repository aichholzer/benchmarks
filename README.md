<div align="center">
<img src="https://github.com/fastify/graphics/raw/master/full-logo.png" width="650" height="auto"/>
</div>

<div align="center">

[![Build Status](https://travis-ci.org/fastify/fastify.svg?branch=master)](https://travis-ci.org/fastify/fastify)
[![Coverage Status](https://coveralls.io/repos/github/fastify/fastify/badge.svg?branch=master)](https://coveralls.io/github/fastify/fastify?branch=master)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](http://standardjs.com/)
[![NPM version](https://img.shields.io/npm/v/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify)
[![NPM downloads](https://img.shields.io/npm/dm/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify) [![Gitter](https://badges.gitter.im/gitterHQ/gitter.svg)](https://gitter.im/fastify)
</div>
<br />

# TL;DR

* [Fastify](https://github.com/fastify/fastify) is, fast and low overhead web framework for Node.js
* This package shows how fast it is comparatively.

# Installing

```
npm i -g fastify-benchmarks
```

# Usage

```
benchmark [arguments (optional)]
```

#### Arguments

* `-h`: Help on how to use the tool.
* `compare`: Get comparative data for your benchmarks.

> You may also compare all test results, at once, in a single table; `benchmark compare -t`

> You can also extend the comparsion table with percentage values based on fastest result; `benchmark compare -p`

# Benchmarks

* __Machine:__ MacBook Pro (Late 2016 | 2,7 GHz Intel Core i7 | 16 GB 2133 MHz LPDDR3)
* __Method:__ `autocannon -c 100 -d 5 -p 10 localhost:3000` (two rounds; one warm-up, one to measure).
* __Node:__ `10.13.0`

| | Version | Router | Requests\/s | Latency | Throughput\/Mb |
| :--- | :-: | :-: | :-: | :-: | --: |
| bare | 10.13.0 | ✗ | 42497.6 | 2.28 | 6.03 |
| connect-router | 1.3.2 | ✓ | 32718.4 | 2.98 | 4.63 |
| connect | 3.6.6 | ✗ | 39164.81 | 2.48 | 5.58 |
| egg.js |  | ✓ | 16954.41 | 5.8 | 5.63 |
| express-route-prefix | 4.16.3 | ✓ | 25009.6 | 3.92 | 8.65 |
| express-with-middlewares | 4.16.3 | ✓ | 20068.8 | 4.87 | 7.30 |
| express | 4.16.3 | ✓ | 26654.4 | 3.66 | 4.20 |
| fastify-big-json | 1.6.0 | ✓ | 7956.8 | 12.31 | 91.60 |
| fastify | 1.6.0 | ✓ | 43804.8 | 2.22 | 6.83 |
| foxify | 0.10.6 | ✓ | 45264 | 2.14 | 6.42 |
| hapi | 17.5.1 | ✓ | 28699.2 | 3.41 | 4.47 |
| koa-router | 7.4.0 | ✓ | 31416 | 3.1 | 4.86 |
| koa | 2.5.1 | ✗ | 34750.4 | 2.8 | 5.47 |
| micro-route | 2.5.0 | ✓ | 34622.4 | 2.81 | 5.44 |
| micro | 9.3.2 | ✗ | 35123.2 | 2.77 | 5.46 |
| microrouter | 3.1.3 | ✓ | 25940.8 | 3.76 | 4.14 |
| polka | 0.4.0 | ✓ | 43158.4 | 2.25 | 6.08 |
| rayo | 1.0.4 | ✓ | 44668.8 | 2.17 | 4.97 |
| restify | 7.2.1 | ✓ | 26945.6 | 3.47 | 4.28 |
| server-base-router | 6.0.0 | ✓ | 44252.8 | 2.19 | 4.97 |
| server-base | 6.0.0 | ✗ | 43177.6 | 2.25 | 4.83 |
| spirit-router | 0.5.0 | ✓ | 32124.8 | 2.9 | 5.03 |
| spirit | 0.6.1 | ✗ | 36726.4 | 2.51 | 5.72 |
| take-five | 1.4.0 | ✓ | 23025.6 | 4 | 7.63 |
| total.js | 2.9.4 | ✓ | 26945.6 | 3.62 | 7.60 |
| trek-engine | 1.0.5 | ✗ | 37462.4 | 2.6 | 5.28 |
| trek-router | 1.2.0 | ✓ | 37339.2 | 2.61 | 5.33 |
| vapr | 0.5.1 | ✓ | 35464 | 2.74 | 5.03 |
