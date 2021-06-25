---
layout: default
title: "sass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sass">
  <a href="/pl/common/sass.html">sass</a> <a href="#sass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konwertuje pliki SCSS lub Sass na CSS.
> Więcej informacji: <https://sass-lang.com/documentation/cli/dart-sass>.

#### Konwertuj plik SCSS lub Sass do CSS i wypisz wynik:
```shell
sass {{plikwejsciowy.scss|plikwejsciowy.sass}}
```
#### Konwertuj plik SCSS lub Sass do CSS i zapisz wynik w pliku:
```shell
sass {{plikwejsciowy.scss|plikwejsciowy.sass}} {{plikwyjsciowy.css}}
```
#### Obejrzyj zmiany w pliku SCSS lub Sass i wyślij lub zaktualizuj plik CSS o tej samej nazwie:
```shell
sass --watch {{plikwejsciowy.scss|plikwejsciowy.sass}}
```
#### Obejrzyj zmiany w pliku SCSS lub Sass i wyślij lub zaktualizuj plik CSS o podanej nazwie:
```shell
sass --watch {{plikwejsciowy.scss|plikwejsciowy.sass}}:{{plikwyjsciowy.css}}
```
{% endraw %}