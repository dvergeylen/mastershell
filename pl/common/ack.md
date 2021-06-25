---
layout: default
title: "ack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ack">
  <a href="/pl/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie wyszukiwania, takie jak grep, zoptymalizowane dla programistów.
> Więcej informacji: <https://beyondgrep.com/documentation/>.

#### Znajdź pliki zawierające „foo”:
```shell
ack {{foo}}
```
#### Znajdź pliki określonego typu:
```shell
ack --ruby {{foo}}
```
#### Policz całkowitą liczbę dopasowań dla terminu „foo”:
```shell
ack -ch {{foo}}
```
#### Pokaż nazwy plików zawierające „foo” i liczbę dopasowań w każdym pliku:
```shell
ack -cl {{foo}}
```
#### Przeszukaj plik pod kątem określonego ciągu znaków:
```shell
ack bar "{{foo bar}}" {{scieżka/do/pliku_lub_katalogu}}
```
#### Przeszukaj plik pod kątem określonego wzorca wyrażenia regularnego:
```shell
ack bar "{{[bB]ar \d+}}" {{scieżka/do/pliku_lub_katalogu}}
```
#### Wypisz wszystkie prawidłowe typy:
```shell
ack --help-types
```
{% endraw %}