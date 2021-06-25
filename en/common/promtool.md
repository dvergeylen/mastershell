---
layout: default
title: "promtool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="promtool">
  <a href="/en/common/promtool.html">promtool</a> <a href="#promtool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tooling for the Prometheus monitoring system.
> More information: <https://prometheus.io/docs/prometheus/latest/getting_started/>.

#### Check if the config files are valid or not (if present report errors):
```shell
promtool check config {{config_file.yml}}
```
#### Check if the rule files are valid or not (if present report errors):
```shell
promtool check rules {{rules_file.yml}}
```
#### Pass Prometheus metrics over stdin to check them for consistency and correctness:
```shell
curl --silent {{http://example.com:9090/metrics/}} | promtool check metrics
```
#### Unit tests for rules config:
```shell
promtool test rules {{test_file.yml}}
```
{% endraw %}