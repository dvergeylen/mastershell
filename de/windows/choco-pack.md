---
layout: default
title: "choco pack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-pack">
  <a href="/de/windows/choco-pack.html">choco pack</a> <a href="#choco-pack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verpacke eine NuGet-Spezifikation in eine nupkg-Datei.
> Weitere Informationen: <https://chocolatey.org/docs/commands-pack>.

#### Verpacke eine NuGet-Spezifikation in eine nupkg-Datei:
```shell
choco pack {{pfad/zu/spezifikation}}
```
#### Verpacke eine NuGet-Spezifikation in eine nupkg-Datei und bestimme die Version der ausgegebenen Datei:
```shell
choco pack {{pfad/zu/spezifikation}} --version {{version}}
```
#### Verpacke eine NuGet-Spezifikation in eine nupkg-Datei, welche in einem bestimmten Verzeichnis gespeichert wird:
```shell
choco pack {{pfad/zu/spezifikation}} --output-directory {{pfad/zu/ausgabe_verzeichnis}}
```
{% endraw %}