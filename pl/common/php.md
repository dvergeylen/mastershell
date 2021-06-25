---
layout: default
title: "php"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="php">
  <a href="/pl/common/php.html">php</a> <a href="#php"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfejs wiersza poleceń PHP.
> Więcej informacji: <https://php.net>.

#### Parsuj i uruchom skrypt php:
```shell
php {{plik}}
```
#### Sprawdź składnię skryptu PHP (np. lint):
```shell
php -l {{plik}}
```
#### Uruchom PHP interaktywnie:
```shell
php -a
```
#### Uruchom kod PHP (uwagi: nie używaj znaczników <? ?> ; unikaj podwójnych cudzysłowów z odwrotnym ukośnikiem):
```shell
php -r "{{kod}}"
```
#### uruchom wbudowany serwer PHP w bieżącym katalogu:
```shell
php -S {{host:port}}
```
#### Uzyskaj listę zainstalowanych rozszerzeń PHP:
```shell
php -m
```
#### Wyświetl informacje o bieżącej konfiguracji PHP:
```shell
php -i
```
{% endraw %}