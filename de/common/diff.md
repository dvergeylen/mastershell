---
layout: default
title: "diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diff">
  <a href="/de/common/diff.html">diff</a> <a href="#diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vergleiche Dateien und Verzeichnisse.
> Weitere Informationen: <https://man7.org/linux/man-pages/man1/diff.1.html>.

#### Vergleiche Dateien (Listet jene Veränderungen auf, mit denen `datei1` zu `datei2` wird):
```shell
diff {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Vergleiche Dateien und ignoriere Leerzeichen:
```shell
diff -w {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Vergleiche Dateien und zeige Unterschiede nebeneinander:
```shell
diff -y {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Vergleiche Dateien und zeige Unterschiede in vereinheitlichtem Format (wie in `git diff`):
```shell
diff -u {{pfad/zu/datei1}} {{pfad/zu/datei2}}
```
#### Vergleiche Verzeichnisse rekursiv (zeigt sowohl Namen von unterschiedlichen Dateien/Verzeichnissen, als auch Unterschiede zwischen Dateien):
```shell
diff -r {{altes_verzeichnis}} {{neues_verzeichnis}}
```
#### Vergleiche Verzeichnisse und zeige nur die Namen der Dateien, die unterschiedlich sind:
```shell
diff -rq {{altes_verzeichnis}} {{neues_verzeichnis}}
```
{% endraw %}