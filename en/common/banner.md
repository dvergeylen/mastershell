---
layout: default
title: "banner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="banner">
  <a href="/en/common/banner.html">banner</a> <a href="#banner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print the given argument as a large ASCII art.
> More information: <https://man.archlinux.org/man/banner.1>.

#### Print the text message as a large banner (quotes are optional):
```shell
banner "{{Hello World}}"
```
#### Print the text message as a banner with a width of 50 characters:
```shell
banner -w {{50}} "{{Hello World}}"
```
#### Read text from stdin:
```shell
banner
```
{% endraw %}