---
layout: default
title: "caffeinate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="caffeinate">
  <a href="/de/osx/caffeinate.html">caffeinate</a> <a href="#caffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hindert den Mac daran in den Schlaf-Modus zu gehen.

#### Halte den Mac für 1 Stunde (3600 Sekunden) wach:
```shell
caffeinate -u -t {{3600}}
```
#### Halte den Mac wach, bis ein bestimmter Befehl abgeschlossen ist:
```shell
caffeinate -s {{befehl}}
```
#### Halte den Mac wach, bis `caffeinate` durch Cmd-C beendet wird:
```shell
caffeinate -i
```
{% endraw %}