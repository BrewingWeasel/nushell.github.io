---
title: dfr quantile
categories: |
  lazyframe
version: 0.83.0
lazyframe: |
  Aggregates the columns to the selected quantile.
usage: |
  Aggregates the columns to the selected quantile.
---

# <code>{{ $frontmatter.title }}</code> for lazyframe

<div class='command-title'>{{ $frontmatter.lazyframe }}</div>

## Signature

```> dfr quantile (quantile)```

## Parameters

 -  `quantile`: quantile value for quantile operation

## Examples

quantile value from columns in a dataframe
```shell
> [[a b]; [6 2] [1 4] [4 1]] | dfr into-df | dfr quantile 0.5
╭───┬──────┬──────╮
│ # │  a   │  b   │
├───┼──────┼──────┤
│ 0 │ 4.00 │ 2.00 │
╰───┴──────┴──────╯

```
