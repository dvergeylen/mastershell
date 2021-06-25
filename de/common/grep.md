---
layout: default
title: "grep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="grep">
  <a href="/de/common/grep.html">grep</a> <a href="#grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Findet Ausdrücke in einem Eingabetext.
> Unterstützt einfache Muster und reguläre Ausdrücke.
> Weitere Informationen: <https://www.gnu.org/software/grep/manual/grep.html>.

#### Suche nach einem Ausdruck in einer Datei:
```shell
grep {{ausdruck}} {{pfad/zu/datei}}
```
#### Suche nach einem exakten Ausdruck:
```shell
grep -F {{exakter_ausdruck}} {{pfad/zu/datei}}
```
#### Suche nach Ausdrücken [R]ekursiv im aktuellen Verzeichnis, zeige zugehörige Zeilen[n]ummern und [I]gnoriere Binärdateien:
```shell
grep -RIn {{ausdruck}} .
```
#### Benutze erweiterte reguläre Ausdrücke (unterstützt `?`, `+`, `{}`, `()` und `|`) ohne Beachtung der Groß-, Kleinschreibung:
```shell
grep -Ei {{ausdruck}} {{pfad/zu/datei}}
```
#### Zeige 3 Zeilen Kontext um [C], vor [B] oder nach [A] jedem Ergebnis:
```shell
grep -{{C|B|A}} 3 {{ausdruck}} {{pfad/zu/datei}}
```
#### Gib den Dateinamen mit zugehöriger Zeilennummer für jedes Ergebnis aus:
```shell
grep -Hn {{ausdruck}} {{pfad/zu/datei}}
```
#### Benutze STDIN, anstatt einer Datei:
```shell
echo "input" | grep {{ausdruck}}
```
#### In[v]ertiere das Ergebnis um bestimmte Ausdrücke auszuschließen:
```shell
grep -v {{ausdruck}}
```
{% endraw %}