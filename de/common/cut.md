---
layout: default
title: "cut"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cut">
  <a href="/de/common/cut.html">cut</a> <a href="#cut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Schneide Felder von stdin oder einer Datei aus.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/cut>.

#### Schneide die ersten 16 Zeichen jeder Zeile von stdin aus:
```shell
cut -c {{1-16}}
```
#### Schneide die ersten 16 Zeichen jeder Zeile der angegebenen Datei aus:
```shell
cut -c {{1-16}} {{pfad/zu/datei}}
```
#### Schneide alles ab dem dritten Zeichen bis zum Ende der Zeile aus:
```shell
cut -c {{3-}}
```
#### Schneide das fünfte Feld jeder Zeile aus und nutze den Doppelpunkt als Trennzeichen (standardmäßig Tab):
```shell
cut -d'{{:}}' -f{{5}}
```
#### Schneide das 2. und 10. Feld jeder Zeile aus und nutze Semikolon als Trennzeichen:
```shell
cut -d'{{;}}' -f{{2,10}}
```
#### Schneide alles ab dem dritten Zeichen bis zum Ende der Zeile aus und nutze Leerzeichen als Trennzeichen:
```shell
cut -d'{{ }}' -f{{3-}}
```
{% endraw %}