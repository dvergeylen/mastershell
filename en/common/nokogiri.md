---
layout: default
title: "nokogiri"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nokogiri">
  <a href="/en/common/nokogiri.html">nokogiri</a> <a href="#nokogiri"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An HTML, XML, SAX and Reader parser.
> More information: <https://nokogiri.org>.

#### Parse the contents of a URL or file:
```shell
nokogiri {{url|path/to/file}}
```
#### Parse as a specific type:
```shell
nokogiri {{url|path/to/file}} --type {{xml|html}}
```
#### Load a specific initialisation file before parsing:
```shell
nokogiri {{url|path/to/file}} -C {{path/to/config_file}}
```
#### Parse using a specific encoding:
```shell
nokogiri {{url|path/to/file}} --encoding {{encoding}}
```
#### Validate using a RELAX NG file:
```shell
nokogiri {{url|path/to/file}} --rng {{url|path/to/file}}
```
{% endraw %}