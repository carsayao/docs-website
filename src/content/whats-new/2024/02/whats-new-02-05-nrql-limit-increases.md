---
title: 'NRQL result limits will increase from 2,000 to 5,000'
summary: 'The maximum result limit for NRQL queries is increasing from 2,000 to 5,000'
releaseDate: '2024-02-05'
learnMoreLink: 'https://docs.newrelic.com/docs/query-your-data/nrql-new-relic-query-language/get-started/nrql-syntax-clauses-functions/#sel-limit'
---

NRQL result limits are increasing from 2,000 to 5,000 results. This increase lets you pull even more data with the `LIMIT` clause when you create NRQL queries, dashboards, and more.

* This change also affects the  `LIMIT MAX` clause, increasing posted results from 2,000 to 5,000.
* If you have an existing query that uses the `LIMIT MAX` clause, your results now reflect the 5,000 limit, assuming the underlying data is populous enough.
* Some existing queries that successfully posted results with `LIMIT MAX` may fail. Larger limits can cause timeouts, or result in failure due to complexity.
* You can use `LIMIT 2000` instead of `LIMIT MAX` to only display 2,000 results.  

This change won't affect existing queries if they lack a `LIMIT` clause, use default result limits, or specify an explicit result below 2,000. 
