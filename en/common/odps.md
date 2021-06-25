---
layout: default
title: "odps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="odps">
  <a href="/en/common/odps.html">odps</a> <a href="#odps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aliyun ODPS (Open Data Processing Service) command-line tool.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

#### Start the command-line with a custom configuration file:
```shell
odpscmd --config={{odps_config.ini}}
```
#### Switch current project:
```shell
use {{project_name}};
```
#### Show tables in the current project:
```shell
show tables;
```
#### Describe a table:
```shell
desc {{table_name}};
```
#### Show table partitions:
```shell
show partitions {{table_name}};
```
#### Describe a partition:
```shell
desc {{table_name}} partition ({{partition_spec}});
```
{% endraw %}