---
layout: default
title: "siege"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="siege">
  <a href="/en/common/siege.html">siege</a> <a href="#siege"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> HTTP loadtesting and benchmarking tool.
> More information: <https://www.joedog.org/siege-manual/>.

#### Test a URL with default settings:
```shell
siege {{https://example.com}}
```
#### Test a list of URLs:
```shell
siege --file {{path/to/url_list.txt}}
```
#### Test list of URLs in a random order (Simulates internet traffic):
```shell
siege --internet --file {{path/to/url_list.txt}}
```
#### Benchmark a list of URLs (without waiting between requests):
```shell
siege --benchmark --file {{path/to/url_list.txt}}
```
#### Set the amount of concurrent connections:
```shell
siege --concurrent={{50}} --file {{path/to/url_list.txt}}
```
#### Set how long for the siege to run for:
```shell
siege --time={{30s}} --file {{path/to/url_list.txt}}
```
{% endraw %}