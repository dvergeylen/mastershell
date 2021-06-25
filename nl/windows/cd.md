---
layout: default
title: "cd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cd">
  <a href="/nl/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Geeft de naam van de huidige werkmap weer of wijzigt deze.
> Meer informatie: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### Ga naar een directory in dezelfde drive:
```shell
cd {{pad/naar/directory}}
```
#### Geef de naam van de huidige directory weer:
```shell
cd
```
#### Ga naar de ouder van de huidige directory:
```shell
cd ..
```
#### Ga naar een directory in een andere drive:
```shell
cd {{pad/naar/directory}} /d
```
{% endraw %}