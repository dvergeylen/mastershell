---
layout: default
title: "xpdf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xpdf">
  <a href="/en/common/xpdf.html">xpdf</a> <a href="#xpdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Portable Document Format (PDF) file viewer.
> More information: <https://www.xpdfreader.com/xpdf-man.html>.

#### Open a PDF file:
```shell
xpdf {{path/to/file.pdf}}
```
#### Open a specific page in a PDF file:
```shell
xpdf {{path/to/file.pdf}} :{{page_number}}
```
#### Open a compressed PDF file:
```shell
xpdf {{path/to/file.pdf.tar}}
```
#### Open a PDF file in fullscreen mode:
```shell
xpdf -fullscreen {{path/to/file.pdf}}
```
#### Specify the initial zoom:
```shell
xpdf -z {{75}}% {{path/to/file.pdf}}
```
#### Specify the initial zoom at page width or full page:
```shell
xpdf -z {{page|width}} {{path/to/file.pdf}}
```
{% endraw %}