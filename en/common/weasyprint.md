---
layout: default
title: "weasyprint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="weasyprint">
  <a href="/en/common/weasyprint.html">weasyprint</a> <a href="#weasyprint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Render HTML to PDF or PNG.
> More information: <https://weasyprint.org/>.

#### Render a HTML file to PDF:
```shell
weasyprint {{path/to/input.html}} {{path/to/output}}.pdf
```
#### Render a HTML file to PNG, including an additional user stylesheet:
```shell
weasyprint {{path/to/input.html}} {{path/to/output}}.png --stylesheet {{path/to/stylesheet.css}}
```
#### Output additional debugging information when rendering:
```shell
weasyprint {{path/to/input.html}} {{path/to/output}}.pdf --verbose
```
#### Specify a custom resolution when outputting to PNG:
```shell
weasyprint {{path/to/input.html}} {{path/to/output}}.png --resolution {{300}}
```
#### Specify a base URL for relative URLs in the input HTML file:
```shell
weasyprint {{path/to/input.html}} {{path/to/output}}.png --base-url {{url_or_filename}}
```
{% endraw %}