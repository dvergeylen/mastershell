---
layout: default
title: "ab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ab">
  <a href="/de/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache HTTP server Benchmarking Tool.
> Weitere Informationen: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Sende 100 HTTP GET Anfragen an eine URL:
```shell
ab -n {{100}} {{url}}
```
#### Sende 100 HTTP GET Anfragen an eine URL, wovon bis zu 10 gleichzeitig bearbeitet werden:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Wach halten:
```shell
ab -k {{url}}
```
#### Lege die maximale Anzahl an Sekunden fest, die das Benchmarking dauern darf:
```shell
ab -t {{60}} {{url}}
```
#### Sende 100 HTTP POST Anfragen an eine URL, wobei eine JSON Belastung aus einer Datei verwendet wird:
```shell
ab -n {{100}} -T {{application/json}} -p {{pfad/zu/datei.json}} {{url}}
```
{% endraw %}