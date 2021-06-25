---
layout: default
title: "echo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="echo">
  <a href="/de/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gib angegebene Argumente aus.
> Weitere Informationen: <https://www.gnu.org/software/coreutils/echo>.

#### Gib einen Text aus. (Hinweis: Anführungszeichen sind optional):
```shell
echo "{{Hallo Welt}}"
```
#### Gib einen Text mit Umgebungsvariablen aus:
```shell
echo "{{Liste aller Systempfade: $PATH}}"
```
#### Gib einen Text ohne darauffolgenden Zeilenumbruch aus:
```shell
echo -n "{{Hallo Welt}}"
```
#### Füge einen Text in eine Datei ein:
```shell
echo "{{Hallo Welt}}" >> {{datei.txt}}
```
#### Ermögliche Interpretation von Fluchtsymbolen (backslash escape):
```shell
echo -e "{{Spalte 1\tSpalte 2}}"
```
{% endraw %}