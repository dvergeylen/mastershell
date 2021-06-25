---
layout: default
title: "hive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hive">
  <a href="/en/common/hive.html">hive</a> <a href="#hive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI tool for Apache Hive.
> More information: <https://cwiki.apache.org/confluence/display/Hive/LanguageManual+Cli>.

#### Start a Hive interactive shell:
```shell
hive
```
#### Run HiveQL:
```shell
hive -e "{{hiveql_query}}"
```
#### Run a HiveQL file with a variable substitution:
```shell
hive --define {{key}}={{value}} -f {{path/to/file.sql}}
```
#### Run a HiveQL with HiveConfig (e.g. `mapred.reduce.tasks=32`):
```shell
hive --hiveconf {{conf_name}}={{conf_value}}
```
{% endraw %}