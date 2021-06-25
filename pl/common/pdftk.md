---
layout: default
title: "pdftk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdftk">
  <a href="/pl/common/pdftk.html">pdftk</a> <a href="#pdftk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zestaw narzędzi PDF.
> Więcej informacji: <https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit>.

#### Wyodrębnij strony 1-3, 5 i 6-10 z pliku PDF oraz zapisz je jako inny plik PDF:
```shell
pdftk {{plik_wejściowy.pdf}} cat {{1-3 5 6-10}} output {{plik_wyjściowy.pdf}}
```
#### Połącz listę plików PDF i zapisz połączony plik jako:
```shell
pdftk {{plik1.pdf plik2.pdf ...}} cat output {{plik_wyjściowy.pdf}}
```
#### Podziel każdą stronę pliku PDF do osobnych plików, o nazwie nadanej według zdefiniowanego wzoru:
```shell
pdftk {{plik_wejściowy.pdf}} burst output {{plik_wyjściowy_%d.pdf}}
```
#### Obróć wszystkie strony o 180 stopni zgodnie ze wskazówkami zegara:
```shell
pdftk {{plik_wejściowy.pdf}} cat {{1-endsouth}} output {{plik_wyjściowy.pdf}}
```
#### Obóć trzecią stronę o 90 stopni zgodnie ze wskazówkami zegara oraz pozostaw pozostałe strony bez zmian:
```shell
pdftk {{plik_wejściowy.pdf}} cat {{1-2 3east 4-end}} output {{plik_wyjściowy.pdf}}
```
{% endraw %}