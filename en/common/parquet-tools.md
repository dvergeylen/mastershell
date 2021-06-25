---
layout: default
title: "parquet-tools"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="parquet-tools">
  <a href="/en/common/parquet-tools.html">parquet-tools</a> <a href="#parquet-tools"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to show, inspect and manipulate Parquet file.
> More information: <https://github.com/apache/parquet-mr/tree/master/parquet-tools>.

#### Display the content of a Parquet file:
```shell
parquet-tools cat {{path/to/parquet}}
```
#### Display the first few lines of a Parquet file:
```shell
parquet-tools head {{path/to/parquet}}
```
#### Print the schema of a Parquet file:
```shell
parquet-tools schema {{path/to/parquet}}
```
#### Print the metadata of a Parquet file:
```shell
parquet-tools meta {{path/to/parquet}}
```
#### Print the content and metadata of a Parquet file:
```shell
parquet-tools dump {{path/to/parquet}}
```
#### Concatenate several Parquet files into the target one:
```shell
parquet-tools merge {{path/to/parquet1}} {{path/to/parquet2}} {{path/to/target_parquet}}
```
#### Print the count of rows in a Parquet file:
```shell
parquet-tools rowcount {{path/to/parquet}}
```
#### Print the column and offset indexes of a Parquet file:
```shell
parquet-tools column-index {{path/to/parquet}}
```
{% endraw %}