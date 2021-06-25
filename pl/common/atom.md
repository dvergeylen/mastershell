---
layout: default
title: "atom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atom">
  <a href="/pl/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wieloplatformowy edytor tekstu z obsługą wtyczek.
> Wtyczkami zarządza się poprzez `apm`.
> Więcej informacji: <https://atom.io/>.

#### Otwórz plik lub katalog:
```shell
atom {{sciezka/do/pliku_lub_katalogu}}
```
#### Otwórz plik lub katalog w nowym oknie:
```shell
atom -n {{sciezka/do/pliku_lub_katalogu}}
```
#### Otwórz plik lub katalog w istniejącym oknie:
```shell
atom --add {{sciezka/do/pliku_lub_katalogu}}
```
#### Otwórz Atom w trybie bezpiecznym (nie ładuje żadnych dodatkowych pakietów):
```shell
atom --safe
```
#### Zapobiega rozwidlaniu się w tle, utrzymuje Atom podłączony do terminala:
```shell
atom --foreground
```
#### Poczekaj na zamknięcie okna Atom przed powrotem (przydatne dla Git commit editor):
```shell
atom --wait
```
{% endraw %}