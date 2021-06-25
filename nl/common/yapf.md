---
layout: default
title: "yapf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yapf">
  <a href="/nl/common/yapf.html">yapf</a> <a href="#yapf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python stijlgidschecker.
> Meer informatie: <https://github.com/google/yapf>.

#### Print de geformateerde diff die zal optreden uit:
```shell
yapf --diff {{pad/naar/bestand}}
```
#### Print de geformateerde diff uit en breng de wijzigingen aan in het bestand:
```shell
yapf --diff --in-place {{pad/naar/bestand}}
```
#### Formatteer alle Python-bestanden recursief in een map in parallel:
```shell
yapf --recursive --in-place --style {{pep8}} --parallel {{pad/naar/map}}
```
{% endraw %}