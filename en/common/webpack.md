---
layout: default
title: "webpack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="webpack">
  <a href="/en/common/webpack.html">webpack</a> <a href="#webpack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bundle a web project's js files and other assets into a single output file.
> More information: <https://webpack.js.org>.

#### Create a single output file from an entry point file:
```shell
webpack {{app.js}} {{bundle.js}}
```
#### Load css files too from the js file (this uses the css loader for `.css` files):
```shell
webpack {{app.js}} {{bundle.js}} --module-bind 'css=css'
```
#### Pass a config file (with eg. the entry script and the output filename) and show compilation progress:
```shell
webpack --config {{webpack.config.js}} --progress
```
#### Automatically recompile on changes to project files:
```shell
webpack --watch {{app.js}} {{bundle.js}}
```
{% endraw %}