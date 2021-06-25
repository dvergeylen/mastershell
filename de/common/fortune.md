---
layout: default
title: "fortune"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fortune">
  <a href="/de/common/fortune.html">fortune</a> <a href="#fortune"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gib ein zufälliges Glückskeks-Zitat aus.
> Weitere Informationen: <https://man.archlinux.org/man/fortune.6>.

#### Gib ein Zitat aus:
```shell
fortune
```
#### Gib ein beleidigendes Zitat aus:
```shell
fortune -o
```
#### Gib ein langes Zitat aus:
```shell
fortune -l
```
#### Gib ein kurzes Zitat aus:
```shell
fortune -s
```
#### Gib alle verfügbaren Zitat-Datenbank-Dateien aus:
```shell
fortune -f
```
#### Gib ein Zitat von einer durch `fortune -f` aufgelisteten Datenbank-Dateien aus:
```shell
fortune {{dateiname}}
```
{% endraw %}