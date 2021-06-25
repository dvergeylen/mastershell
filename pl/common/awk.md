---
layout: default
title: "awk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="awk">
  <a href="/pl/common/awk.html">awk</a> <a href="#awk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wszechstronny język programowania do pracy na plikach.
> Więcej informacji: <https://github.com/onetrueawk/awk>.

#### Wydrukuj piątą kolumnę (aka. pole) w pliku oddzielonym spacjami:
```shell
awk '{print $5}' {{nazwapliku}}
```
#### Wydrukuj drugą kolumnę wierszy zawierających "something" w pliku oddzielonym spacjami:
```shell
awk '/{{coś}}/ {print $2}' {{nazwapliku}}
```
#### Wydrukuj ostatnią kolumnę każdego wiersza w pliku, używając przecinka (zamiast spacji) jako separatora pola:
```shell
awk -F ',' '{print $NF}' {{nazwapliku}}
```
#### Zsumuj wartości w pierwszej kolumnie pliku i wydrukuj sumę:
```shell
awk '{s+=$1} END {print s}' {{nazwapliku}}
```
#### Zsumuj wartości w pierwszej kolumnie i wydrukuj wartości, a następnie sumę:
```shell
awk '{s+=$1; print $1} END {print "--------"; print s}' {{nazwapliku}}
```
#### Drukuj co trzeci wiersz, zaczynając od pierwszego wiersza:
```shell
awk 'NR%3==1' {{nazwapliku}}
```
#### Wydrukuj wszystkie wartości, zaczynając od trzeciej kolumny:
```shell
awk '{for (i=3; i <= NF; i++) printf $i""FS; print""}' {{nazwapliku}}
```
#### Wydrukuj różne wartości w zależności od warunków:
```shell
awk '{if ($1 == "foo") print "Dokładne dopasowanie foo"; else if ($1 ~ "bar") print "Częściowe dopasowanie bar"; else print "Baz"}' {{nazwapliku}}
```
{% endraw %}