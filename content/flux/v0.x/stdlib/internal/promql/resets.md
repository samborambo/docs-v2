---
title: promql.resets() function
description: >
  `promql.resets()` implements functionality equivalent to
  [PromQL's `resets()` function](https://prometheus.io/docs/prometheus/latest/querying/functions/#resets).
menu:
  flux_0_x_ref:
    name: promql.resets
    parent: internal/promql
    identifier: internal/promql/resets
weight: 201
---

<!------------------------------------------------------------------------------

IMPORTANT: This page was generated from comments in the Flux source code. Any
edits made directly to this page will be overwritten the next time the
documentation is generated. 

To make updates to this documentation, update the function comments above the
function definition in the Flux source code:

https://github.com/influxdata/flux/blob/master/stdlib/internal/promql/promql.flux#L170-L170

Contributing to Flux: https://github.com/influxdata/flux#contributing
Fluxdoc syntax: https://github.com/influxdata/flux/blob/master/docs/fluxdoc.md

------------------------------------------------------------------------------->

`promql.resets()` implements functionality equivalent to
[PromQL's `resets()` function](https://prometheus.io/docs/prometheus/latest/querying/functions/#resets).



##### Function type signature

```js
(<-tables: stream[{A with _value: float}]) => stream[{B with _value: float}]
```

{{% caption %}}For more information, see [Function type signatures](/flux/v0.x/function-type-signatures/).{{% /caption %}}

## Parameters

### tables

Input data. Defaults is piped-forward data (`<-`).



