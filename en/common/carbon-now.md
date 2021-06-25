---
layout: default
title: "carbon-now"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="carbon-now">
  <a href="/en/common/carbon-now.html">carbon-now</a> <a href="#carbon-now"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create beautiful images of code.
> More information: <https://github.com/mixn/carbon-now-cli>.

#### Create an image from a file using default settings:
```shell
carbon-now {{file}}
```
#### Create an image from a text in clipboard using default settings:
```shell
carbon-now --from-clipboard
```
#### Create an image from standard input using default settings:
```shell
{{input}} | carbon-now
```
#### Create images interactively for custom settings and optionally save a preset:
```shell
carbon-now -i {{file}}
```
#### Create images from previously saved preset:
```shell
carbon-now -p {{preset}} {{file}}
```
#### Start at a specified line of text:
```shell
carbon-now -s {{line}} {{file}}
```
#### End at a specific line of text:
```shell
carbon-now -e {{line}} {{file}}
```
#### Open image in a browser instead of saving:
```shell
carbon-now --open {{file}}
```
{% endraw %}