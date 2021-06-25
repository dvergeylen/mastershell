---
layout: default
title: "decaffeinate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="decaffeinate">
  <a href="/en/common/decaffeinate.html">decaffeinate</a> <a href="#decaffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Move your CoffeeScript source to modern JavaScript.
> More information: <https://decaffeinate-project.org>.

#### Convert a CoffeeScript file to JavaScript:
```shell
decaffeinate {{path/to/file.coffee}}
```
#### Convert a CoffeeScript v2 file to JavaScript:
```shell
decaffeinate --use-cs2 {{path/to/file.coffee}}
```
#### Convert require and `module.exports` to import and export:
```shell
decaffeinate --use-js-modules {{path/to/file.coffee}}
```
#### Convert a CoffeeScript, allowing named exports:
```shell
decaffeinate --loose-js-modules {{path/to/file.coffee}}
```
{% endraw %}