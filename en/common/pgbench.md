---
layout: default
title: "pgbench"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pgbench">
  <a href="/en/common/pgbench.html">pgbench</a> <a href="#pgbench"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a benchmark test on PostgreSQL.
> More information: <https://www.postgresql.org/docs/10/pgbench.html>.

#### Initialize a database with a scale factor of 50 times the default size:
```shell
pgbench --initialize --scale={{50}} {{database_name}}
```
#### Benchmark a database with 10 clients, 2 worker threads, and 10,000 transactions per client:
```shell
pgbench --client={{10}} --jobs={{2}} --transactions={{10000}} {{database_name}}
```
{% endraw %}