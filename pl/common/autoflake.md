---
layout: default
title: "autoflake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autoflake">
  <a href="/pl/common/autoflake.html">autoflake</a> <a href="#autoflake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie do usuwania nieużywanych importów i zmiennych z kodu Python.
> Więcej informacji: <https://github.com/myint/autoflake>.

#### Usuń nieużywane zmienne z jednego pliku i wyświetl różnicę:
```shell
autoflake --remove-unused-variables {{file.py}}
```
#### Usuń nieużywane importy z wielu plików i wyświetl różnice:
```shell
autoflake --remove-all-unused-imports {{file1.py}} {{file2.py}} {{file3.py}}
```
#### Usuń nieużywane zmienne z pliku, zastępując plik:
```shell
autoflake --remove-unused-variables --in-place {{file.py}}
```
#### Usuń nieużywane zmienne rekurencyjnie ze wszystkich plików w katalogu, nadpisując każdy plik:
```shell
autoflake --remove-unused-variables --in-place --recursive {{sciezka/do/katalogu}}
```
{% endraw %}