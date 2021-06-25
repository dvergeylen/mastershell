---
layout: default
title: "slimrb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="slimrb">
  <a href="/en/common/slimrb.html">slimrb</a> <a href="#slimrb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert Slim files to HTML.

#### Convert a Slim file to HTML:
```shell
slimrb {{input.slim}} {{output.html}}
```
#### Convert a Slim file and output to prettified HTML:
```shell
slimrb --pretty {{input.slim}} {{output.html}}
```
#### Convert a Slim file to ERB:
```shell
slimrb --erb {{input.slim}} {{output.erb}}
```
{% endraw %}