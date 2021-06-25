---
layout: default
title: "rar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rar">
  <a href="/pl/common/rar.html">rar</a> <a href="#rar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiwizator RAR. Obsługuje wielotomowe archiwa, które mogą być opcjonalnie samorozpakowujące się.

#### Zarchiwizuj 1 lub więcej plików:
```shell
rar a {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik1}} {{sciezka/do/plik2}} {{sciezka/do/plik3}}
```
#### Zarchiwizuj katalog:
```shell
rar a {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/katalog}}
```
#### Podziel archiwum na części równej wielkości (50M):
```shell
rar a -v{{50M}} -R {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik_lub_katalog}}
```
#### Chroń hasło wynikowego archiwum:
```shell
rar a -p{{haslo}} {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik_lub_katalog}}
```
#### Szyfruj dane pliku i nagłówki za pomocą hasła:
```shell
rar a -hp{{haslo}} {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik_lub_katalog}}
```
#### Użyj określonego poziomu kompresji (0-5):
```shell
rar a -m{{poziom_kompresji}} {{sciezka/do/nazwa_archiwum.rar}} {{sciezka/do/plik_lub_katalog}}
```
{% endraw %}