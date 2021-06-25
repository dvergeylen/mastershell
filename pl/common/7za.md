---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/pl/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiwizator plików o wysokim współczynniku kompresji.
> Samodzielna wersja `7z` z obsługą mniejszej liczby typów archiwów.
> Więcej informacji: <https://www.7-zip.org/>.

#### Zarchiwizuj plik lub katalog:
```shell
7za a {{archiwum.7z}} {{scieżka/do/pliku_lub_katalogu}}
```
#### Wyodrębnij istniejący plik 7z z oryginalną strukturą katalogów:
```shell
7za x {{archiwum}}
```
#### Zarchiwizuj przy użyciu określonego typu archiwum:
```shell
7za a -t{{zip|gzip|bzip2|tar}} {{archiwum}} {{scieżka/do/pliku_lub_katalogu}}
```
#### Wypisz dostępe typy archiwów:
```shell
7za i
```
#### Wypisz zawartość pliku archiwum:
```shell
7za l {{archiwum}}
```
{% endraw %}