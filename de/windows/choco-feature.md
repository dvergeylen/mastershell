---
layout: default
title: "choco feature"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-feature">
  <a href="/de/windows/choco-feature.html">choco feature</a> <a href="#choco-feature"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interagiere mit Funktionen, die das Verhalten von Chocolatey verändern.
> Weitere Informationen: <https://chocolatey.org/docs/commands-feature>.

#### Gib eine Liste von verfügbaren Funktionen aus:
```shell
choco feature list
```
#### Aktiviere eine Funktion:
```shell
choco feature enable --name {{name}}
```
#### Deaktiviere eine Funktion:
```shell
choco feature disable --name {{name}}
```
{% endraw %}