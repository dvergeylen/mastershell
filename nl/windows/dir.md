---
layout: default
title: "dir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dir">
  <a href="/nl/windows/dir.html">dir</a> <a href="#dir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geeft de inhoud weer van een directory.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/dir>.

#### Geef de inhoud weer van de huidige map:
```shell
dir
```
#### Geef de inhoud weer van een gegeven directory:
```shell
dir {{pad/naar/directory}}
```
#### Geef de inhoud weer van de huidige directory, inclusief verborgen bestanden:
```shell
dir /A
```
#### Geef de inhoud weer van een gegeven directory, inclusief verborgen bestanden:
```shell
dir {{pad/naar/directory}} /A
```
{% endraw %}