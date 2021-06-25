---
layout: default
title: "inkmake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="inkmake">
  <a href="/en/common/inkmake.html">inkmake</a> <a href="#inkmake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Makefile-style SVG exporting using Inkscape's backend.
> More information: <https://github.com/wader/inkmake>.

#### Export an SVG file executing the specified Inkfile:
```shell
inkmake {{path/to/Inkfile}}
```
#### Execute an Inkfile and show detailed information:
```shell
inkmake --verbose {{path/to/Inkfile}}
```
#### Execute an Inkfile, specifying SVG input file(s) and an output file:
```shell
inkmake --svg {{path/to/file.svg}} --out {{path/to/output_image}} {{path/to/Inkfile}}
```
#### Specify a custom Inkscape binary to use as the backend:
```shell
inkmake --inkscape {{/Applications/Inkscape.app/Contents/Resources/bin/inkscape}} {{path/to/Inkfile}}
```
#### Display help:
```shell
inkmake --help
```
{% endraw %}