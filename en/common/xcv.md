---
layout: default
title: "xcv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcv">
  <a href="/en/common/xcv.html">xcv</a> <a href="#xcv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cut, copy, and paste in the command-line.
> More information: <https://github.com/busterc/xcv>.

#### Cut a file:
```shell
xcv x {{input_file}}
```
#### Copy a file:
```shell
xcv c {{input_file}}
```
#### Paste a file:
```shell
xcv v {{output_file}}
```
#### List files available for pasting:
```shell
xcv l
```
{% endraw %}