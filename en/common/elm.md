---
layout: default
title: "elm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="elm">
  <a href="/en/common/elm.html">elm</a> <a href="#elm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile and run Elm source files.
> More information: <https://elm-lang.org>.

#### Initialize an Elm project, generates an elm.json file:
```shell
elm init
```
#### Start interactive Elm shell:
```shell
elm repl
```
#### Compile an Elm file, output the result to an `index.html` file:
```shell
elm make {{source}}
```
#### Compile an Elm file, output the result to a JavaScript file:
```shell
elm make {{source}} --output={{destination}}.js
```
#### Start local web server that compiles Elm files on page load:
```shell
elm reactor
```
#### Install Elm package from https://package.elm-lang.org:
```shell
elm install {{author}}/{{package}}
```
{% endraw %}