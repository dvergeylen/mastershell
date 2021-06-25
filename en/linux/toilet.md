---
layout: default
title: "toilet"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="toilet">
  <a href="/en/linux/toilet.html">toilet</a> <a href="#toilet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to display ASCII-art fonts.
> More information: <http://caca.zoy.org/wiki/toilet>.

#### Generate ASCII art for a given text:
```shell
toilet {{input_text}}
```
#### Generate ASCII art using a custom font file:
```shell
toilet {{input_text}} -f {{font_filename}}
```
#### Generate ASCII art using a filter:
```shell
toilet {{input_text}} --filter {{filter_name}}
```
#### Show available toilet filters:
```shell
toilet --filter list 
```
{% endraw %}