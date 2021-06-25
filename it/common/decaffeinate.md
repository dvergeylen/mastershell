---
layout: default
title: "decaffeinate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="decaffeinate">
  <a href="/it/common/decaffeinate.html">decaffeinate</a> <a href="#decaffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converti script CoffeScript in JavaScript moderno.
> Maggiori informazioni: <https://decaffeinate-project.org>.

#### Converti un file CoffeeScript in JavaScript:
```shell
decaffeinate {{percorso/al/file.coffee}}
```
#### Converti un file CoffeeScript v2 in JavaScript:
```shell
decaffeinate --use-cs2 {{percorso/al/file.coffee}}
```
#### Converti `require` e `module.exports` in `import` ed `export`:
```shell
decaffeinate --use-js-modules {{percorso/al/file.coffee}}
```
#### Converti un file CoffeeScript, permettendo di esportare nomi:
```shell
decaffeinate --loose-js-modules {{percorso/al/file.coffee}}
```
{% endraw %}