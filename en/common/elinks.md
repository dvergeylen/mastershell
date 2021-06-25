---
layout: default
title: "elinks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="elinks">
  <a href="/en/common/elinks.html">elinks</a> <a href="#elinks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text based browser similar to lynx.
> More information: <http://elinks.or.cz>.

#### Start elinks:
```shell
elinks
```
#### Quit elinks:
```shell
Ctrl + C
```
#### Dump output of webpage to console, colorizing the text with ANSI control codes:
```shell
elinks -dump -dump-color-mode {{1}} {{url}}
```
{% endraw %}