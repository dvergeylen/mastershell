---
layout: default
title: "vegeta"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vegeta">
  <a href="/en/common/vegeta.html">vegeta</a> <a href="#vegeta"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line utility and a library for HTTP load testing.
> See also `ab`.
> More information: <https://github.com/tsenart/vegeta>.

#### Launch an attack lasting 30 seconds:
```shell
echo "{{GET https://example.com}}" | vegeta attack -duration={{30s}}
```
#### Launch an attack on a server with a self-signed https certificate:
```shell
echo "{{GET https://example.com}}" | vegeta attack -insecure -duration={{30s}}
```
#### Launch an attack with a rate of 10 requests per second:
```shell
echo "{{GET https://example.com}}" | vegeta attack -duration={{30s}} -rate={{10}}
```
#### Launch an attack and display a report:
```shell
echo "{{GET https://example.com}}" | vegeta attack -duration={{30s}} | vegeta report
```
#### Launch an attack and plot the results on a graph (latency over time):
```shell
echo "{{GET https://example.com}}" | vegeta attack -duration={{30s}} | vegeta plot > {{path/to/results.html}}
```
#### Launch an attack against multiple URLs from a file:
```shell
vegeta attack -duration={{30s}} -targets={{requests.txt}} | vegeta report
```
{% endraw %}