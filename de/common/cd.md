---
layout: default
title: "cd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cd">
  <a href="/de/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ändere das aktuelle Arbeitsverzeichnis.
> Weitere Informationen: <https://man.archlinux.org/man/cd.n>.

#### Wechsle in das angegebene Verzeichnis:
```shell
cd {{pfad/zu/verzeichnis}}
```
#### Wechsle in das Home-Verzeichnis des aktuellen Benutzers:
```shell
cd
```
#### Wechsle zum Verzeichnis über dem aktuellen Verzeichnis:
```shell
cd ..
```
#### Wechsle zum zuletzt gewählten Verzeichnis:
```shell
cd -
```
{% endraw %}