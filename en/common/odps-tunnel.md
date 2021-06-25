---
layout: default
title: "odps tunnel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="odps-tunnel">
  <a href="/en/common/odps-tunnel.html">odps tunnel</a> <a href="#odps-tunnel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Data tunnel in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

#### Download table to local file:
```shell
tunnel download {{table_name}} {{file}};
```
#### Upload local file to a table partition:
```shell
tunnel upload {{file}} {{table_name}}/{{partition_spec}};
```
#### Upload table specifying field and record delimiters:
```shell
tunnel upload {{file}} {{table_name}} -fd {{field_delim}} -rd {{record_delim}};
```
#### Upload table using multiple threads:
```shell
tunnel upload {{file}} {{table_name}} -threads {{num}};
```
{% endraw %}