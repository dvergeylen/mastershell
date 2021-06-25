---
layout: default
title: "7zr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7zr">
  <a href="/pl/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiwizator plików o wysokim współczynniku kompresji.
> Samodzielna wersja `7z` obsługująca tylko pliki typu .7z.
> Więcej informacji: <https://www.7-zip.org/>.

#### Zarchiwizuj plik lub katalog:
```shell
7zr a {{archiwum.7z}} {{scieżka/do/pliku_lub_katalogu}}
```
#### Wyodrębnij istniejący plik 7z z oryginalną strukturą katalogów:
```shell
7zr x {{archiwum.7z}}
```
#### Wypisz zawartość pliku archiwum:
```shell
7zr l {{archiwum.7z}}
```
{% endraw %}