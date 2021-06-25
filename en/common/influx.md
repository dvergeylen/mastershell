---
layout: default
title: "influx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="influx">
  <a href="/en/common/influx.html">influx</a> <a href="#influx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> InfluxDB command-line client.
> More information: <https://docs.influxdata.com/influxdb/v1.7/tools/shell/>.

#### Connect to an InfluxDB running on localhost with no credentials:
```shell
influx
```
#### Connect with a specific username (will prompt for a password):
```shell
influx -username {{username}} -password ""
```
#### Connect to a specific host:
```shell
influx -host {{hostname}}
```
#### Use a specific database:
```shell
influx -database {{database_name}}
```
#### Execute a given command:
```shell
influx -execute "{{influxql_command}}"
```
#### Return output in a specific format:
```shell
influx -execute "{{influxql_command}}" -format {{json|csv|column}}
```
{% endraw %}