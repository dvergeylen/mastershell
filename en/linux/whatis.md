---
layout: default
title: "whatis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whatis">
  <a href="/en/linux/whatis.html">whatis</a> <a href="#whatis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display one-line descriptions from manual pages.

#### Display a description from a man page:
```shell
whatis {{command}}
```
#### Don't cut the description off at the end of the line:
```shell
whatis --long {{command}}
```
#### Display descriptions for all commands matching a glob:
```shell
whatis --wildcard {{net*}}
```
#### Search man page descriptions with a regular expression:
```shell
whatis --regex '{{wish[0-9]\.[0-9]}}'
```
{% endraw %}