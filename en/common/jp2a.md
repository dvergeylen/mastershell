---
layout: default
title: "jp2a"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jp2a">
  <a href="/en/common/jp2a.html">jp2a</a> <a href="#jp2a"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert JPEG images to ASCII.
> More information: <https://csl.name/jp2a/>.

#### Read JPEG image from a file and print in ASCII:
```shell
jp2a {{path/to/image.jpeg}}
```
#### Read JPEG image from a URL and print in ASCII:
```shell
jp2a {{www.example.com/image.jpeg}}
```
#### Colorize the ASCII output:
```shell
jp2a --colors {{path/to/image.jpeg}}
```
#### Specify characters to be used for the ASCII output:
```shell
jp2a --chars='{{..-ooxx@@}}' {{path/to/image.jpeg}}
```
#### Write the ASCII output into a file:
```shell
jp2a --output={{path/to/output_file.txt}} {{path/to/image.jpeg}}
```
#### Write the ASCII output in HTML file format, suitable for viewing in web browsers:
```shell
jp2a --html --output={{path/to/output_file.html}} {{path/to/image.jpeg}}
```
{% endraw %}