---
layout: default
title: "scoop bucket"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scoop-bucket">
  <a href="/de/windows/scoop-bucket.html">scoop bucket</a> <a href="#scoop-bucket"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte "Eimer": Git-Repositories, welche Dateien enthalten, die beschreiben, wie Scoop Programme installiert werden.
> Kennt Scoop nicht die URL eines Eimers, so muss diese angegeben werden.
> Weitere Informationen: <https://github.com/lukesampson/scoop/wiki/Buckets>.

#### Liste alle Eimer auf, die gerade aktiv sind:
```shell
scoop bucket list
```
#### Liste alle bekannten Eimer auf:
```shell
scoop bucket known
```
#### Aktiviere einen bekannten Eimer:
```shell
scoop bucket add {{name}}
```
#### Aktiviere einen unbekannten Eimer durch die Angabe eines Namens und einer Git-Repository-URL:
```shell
scoop bucket add {{name}} {{https://beispiel.de/repository.git}}
```
#### Deaktiviere einen Eimer:
```shell
scoop bucket rm {{name}}
```
{% endraw %}