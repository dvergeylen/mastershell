---
layout: default
title: "ul"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ul">
  <a href="/en/linux/ul.html">ul</a> <a href="#ul"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Performs the underlining of a text.
> Each character in a given string must be underlined separately.

#### Display the contents of the file with underlines where applicable:
```shell
ul {{file.txt}}
```
#### Display the contents of the file with underlines made of dashes `-`:
```shell
ul -i {{file.txt}}
```
{% endraw %}