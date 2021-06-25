---
layout: default
title: "asciiart"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asciiart">
  <a href="/en/linux/asciiart.html">asciiart</a> <a href="#asciiart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert images to ASCII.
> More information: <https://github.com/nodanaonlyzuul/asciiart>.

#### Read an image from a file and print in ASCII:
```shell
asciiart {{path/to/image.jpg}}
```
#### Read an image from a URL and print in ASCII:
```shell
asciiart {{www.example.com/image.jpg}}
```
#### Choose the output width (default is 100):
```shell
asciiart -width {{50}} {{path/to/image.jpg}}
```
#### Colorize the ASCII output:
```shell
asciiart --color {{path/to/image.jpg}}
```
#### Choose the output format (default format is text):
```shell
asciiart --format {{text|html}} {{path/to/image.jpg}}
```
#### Invert the character map:
```shell
asciiart --invert-chars {{path/to/image.jpg}}
```
{% endraw %}