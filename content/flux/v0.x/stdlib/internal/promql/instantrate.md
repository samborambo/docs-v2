---
title: promql.instantRate() function
description: >
  `promql.instantRate()` is a helper function that calculates instant rates over
  counters and is used to implement PromQL's
  [`irate()`](https://prometheus.io/docs/prometheus/latest/querying/functions/#irate) and
  [`idelta()`](https://prometheus.io/docs/prometheus/latest/querying/functions/#idelta) functions.
menu:
  flux_0_x_ref:
    name: promql.instantRate
    parent: internal/promql
    identifier: internal/promql/instantRate
weight: 201
---

<!------------------------------------------------------------------------------

IMPORTANT: This page was generated from comments in the Flux source code. Any
edits made directly to this page will be overwritten the next time the
documentation is generated. 

To make updates to this documentation, update the function comments above the
function definition in the Flux source code:

https://github.com/influxdata/flux/blob/master/stdlib/internal/promql/promql.flux#L93-L96

Contributing to Flux: https://github.com/influxdata/flux#contributing
Fluxdoc syntax: https://github.com/influxdata/flux/blob/master/docs/fluxdoc.md

------------------------------------------------------------------------------->

`promql.instantRate()` is a helper function that calculates instant rates over
counters and is used to implement PromQL's
[`irate()`](https://prometheus.io/docs/prometheus/latest/querying/functions/#irate) and
[`idelta()`](https://prometheus.io/docs/prometheus/latest/querying/functions/#idelta) functions.



##### Function type signature

```js
(<-tables: stream[{A with _value: float, _time: time}], ?isRate: bool) => stream[{B with _value: float}]
```

{{% caption %}}For more information, see [Function type signatures](/flux/v0.x/function-type-signatures/).{{% /caption %}}

## Parameters

### tables

Input data. Defaults is piped-forward data (`<-`).



### isRate

Data represents a rate.



