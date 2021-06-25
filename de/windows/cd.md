---
layout: default
title: "cd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cd">
  <a href="/de/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige den Namen des aktuellen Arbeitsverzeichnisses an oder ändere dieses.
> Weitere Informationen: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Wechsle zu einem Verzeichnis im selben Laufwerk:
```shell
cd {{pfad/zu/verzeichnis}}
```
#### Zeige den Namen des aktuellen Verzeichnisses an:
```shell
cd
```
#### Wechsle zum übergeordneten Verzeichnis des aktuellen Verzeichnisses:
```shell
cd ..
```
#### Wechsle in ein Verzeichnis auf einem anderen Laufwerk:
```shell
cd {{pfad/zu/verzeichnis}} /d
```
{% endraw %}