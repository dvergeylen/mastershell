---
layout: default
title: "gedit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gedit">
  <a href="/pt_pt/linux/gedit.html">gedit</a> <a href="#gedit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Editor de texto para Desktop do GNOME.

#### Abrir ficheiro de texto:
```shell
gedit {{ficheiro}}
```
#### Abrir múltiplos ficheiros de texto:
```shell
gedit {{ficheiro1 ficheiro2}}
```
#### Mostrar a lista de formatações de texto disponíveis:
```shell
gedit --list-encodings
```
#### Abrir um ficheiro de texto com uma formatação específica:
```shell
gedit --encoding={{encoding}} {{ficheiro}}
```
{% endraw %}