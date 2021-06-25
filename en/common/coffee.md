---
layout: default
title: "coffee"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="coffee">
  <a href="/en/common/coffee.html">coffee</a> <a href="#coffee"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executes CoffeeScript scripts or compiles them into JavaScript.
> More information: <https://coffeescript.org#cli>.

#### Run a script:
```shell
coffee {{path/to/file.coffee}}
```
#### Compile to JavaScript and save to a file with the same name:
```shell
coffee --compile {{path/to/file.coffee}}
```
#### Compile to JavaScript and save to a given output file:
```shell
coffee --compile {{path/to/file.coffee}} --output {{path/to/file.js}}
```
#### Run interactive REPL:
```shell
coffee --interactive
```
#### Watch script for changes and re-run script:
```shell
coffee --watch {{path/to/file.coffee}}
```
{% endraw %}