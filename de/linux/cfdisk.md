---
layout: default
title: "cfdisk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cfdisk">
  <a href="/de/linux/cfdisk.html">cfdisk</a> <a href="#cfdisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ein Programm zur Verwaltung von Partitionstabellen mittels einer Curses-basierten UI.
> Weitere Informationen: <https://manned.org/cfdisk>.

#### Öffne das Partitionierungsinterface für eine bestimmte Festplatte:
```shell
cfdisk {{/dev/sdX}}
```
#### Erzeuge und bearbeite eine neue Partitionierungstabelle für eine bestimmte Festplatte:
```shell
cfdisk --zero {{/dev/sdX}}
```
{% endraw %}