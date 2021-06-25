---
layout: default
title: "babel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="babel">
  <a href="/pl/common/babel.html">babel</a> <a href="#babel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transpiler, który konwertuje kod ze składni JavaScript ES6 / ES7 na składnię ES5.
> Więcej informacji: <https://babeljs.io/>.

#### Transpiluj określony plik wejściowy i dane wyjściowe do stdout:
```shell
babel {{siezka/do/pliku}}
```
#### Transpiluj określony plik wejściowy i wyjście do określonego pliku:
```shell
babel {{sciezka/do/pliku_wejsciowego}} --out-file {{sciezka/do/pliku_wyjsciowego}}
```
#### Transpiluj plik wejściowy przy każdej zmianie:
```shell
babel {{sciezka/do/pliku_wejsciowego}} --watch
```
#### Transpiluj cały katalog plików:
```shell
babel {{sciezka/do/katalogu_wejsciowego}}
```
#### Zignoruj określone pliki oddzielone przecinkami w katalogu:
```shell
babel {{sciezka/do/katalogu_wejsciowego}} --ignore {{ignorowane_pliki}}
```
#### Transpiluj i wypisz jako zminimalizowany JavaScript:
```shell
babel {{sciezka/do/pliku_wejsciowego}} --minified
```
#### Wybierz zestaw ustawień dla formatowania wyjściowego:
```shell
babel {{sciezka/do/pliku_wejsciowego}} --presets {{presets}}
```
#### Wyświetl wszystkie dostępne opcje:
```shell
babel --help
```
{% endraw %}