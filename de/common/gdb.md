---
layout: default
title: "gdb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gdb">
  <a href="/de/common/gdb.html">gdb</a> <a href="#gdb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Der GNU Debugger.
> Weitere Informationen: <https://www.gnu.org/software/gdb>.

#### Debugge eine ausführbare Datei:
```shell
gdb {{ausführbare_datei}}
```
#### Binde einen Prozess an gdb:
```shell
gdb -p {{prozess_ID}}
```
#### Debugge mit einer Kerndatei:
```shell
gdb -c {{kerndatei}} {{ausführbare_datei}}
```
#### Führe angegebene Befehle beim Start von gdb aus:
```shell
gdb -ex "{{befehle}}" {{ausführbare_datei}}
```
#### Starte gdb und übergib Argumente an die ausführbare Datei:
```shell
gdb --args {{ausführbare_datei}} {{argument1}} {{argument2}}
```
{% endraw %}