---
layout: default
title: "pdfimages"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfimages">
  <a href="/pl/common/pdfimages.html">pdfimages</a> <a href="#pdfimages"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Narzędzie do wyodrębniania obrazów z plików PDF.

#### Wyodrębnij wszystkie obrazy z pliku PDF i zapisz je jako pliki PNG:
```shell
pdfimages -png {{ścieżka/do/pliku.pdf}} {{przedrostek_nazwy_pliku}}
```
#### Wyodrębnij obrazy ze stron 3 do 5:
```shell
pdfimages -f {{3}} -l {{5}} {{ścieżka/do/pliku.pdf}} {{przedrostek_nazwy_pliku}}
```
#### Wyodrębnij obrazy z pliku PDF oraz zawrzyj numer strony w nazwach wyjściowych:
```shell
pdfimages -p {{ścieżka/do/pliku.pdf}} {{przedrostek_nazwy_pliku}}
```
#### Wyświetl listę informacji o każdym obrazie w pliku PDF:
```shell
pdfimages -list {{ścieżka/do/pliku.pdf}}
```
{% endraw %}