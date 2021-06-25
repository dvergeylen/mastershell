---
layout: default
title: "postcss"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="postcss">
  <a href="/en/common/postcss.html">postcss</a> <a href="#postcss"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PostCSS is a tool for transforming styles with JS plugins.
> More information: <https://postcss.org>.

#### Parse and transform a CSS file:
```shell
postcss {{path/to/file}}
```
#### Parse and transform a CSS file and output to a specific file:
```shell
postcss {{path/to/file}} --output {{path/to/file}}
```
#### Parse and transform a CSS file and output to a specific directory:
```shell
postcss {{path/to/file}} --dir {{path/to/directory}}
```
#### Parse and transform a CSS file in-place:
```shell
postcss {{path/to/file}} --replace
```
#### Specify a custom PostCSS parser:
```shell
postcss {{path/to/file}} --parser {{parser}}
```
#### Specify a custom PostCSS syntax:
```shell
postcss {{path/to/file}} --syntax {{syntax}}
```
#### Watch for changes to a CSS file:
```shell
postcss {{path/to/file}} --watch
```
#### Display available options and examples:
```shell
postcss --help
```
{% endraw %}