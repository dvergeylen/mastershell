---
layout: default
title: "amass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="amass">
  <a href="/en/common/amass.html">amass</a> <a href="#amass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> In-depth Attack Surface Mapping and Asset Discovery tool.
> More information: <https://github.com/OWASP/Amass>.

#### Check the Amass version:
```shell
amass -version
```
#### Show general help:
```shell
amass -help
```
#### Show help on an Amass subcommand (like `intel`, `enum`, etc.):
```shell
amass -help {{subcommand}}
```
#### Execute an Amass subcommand:
```shell
amass {{subcommand}}
```
{% endraw %}