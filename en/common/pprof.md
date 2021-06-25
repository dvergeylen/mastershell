---
layout: default
title: "pprof"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pprof">
  <a href="/en/common/pprof.html">pprof</a> <a href="#pprof"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool for visualization and analysis of profile data.
> More information: <https://github.com/google/pprof>.

#### Generate a text report from a specific profiling file, on fibbo binary:
```shell
pprof -top {{./fibbo}} {{./fibbo-profile.pb.gz}}
```
#### Generate a graph and open it on a web browser:
```shell
pprof -svg {{./fibbo}} {{./fibbo-profile.pb.gz}}
```
#### Run pprof in interactive mode to be able to manually launch `pprof` on a file:
```shell
pprof {{./fibbo}} {{./fibbo-profile.pb.gz}}
```
#### Run a web server that serves a web interface on top of `pprof`:
```shell
pprof -http={{localhost:8080}} {{./fibbo}} {{./fibbo-profile.pb.gz}}
```
#### Fetch a profile from an HTTP server and generate a report:
```shell
pprof {{http://localhost:8080/debug/pprof}}
```
{% endraw %}