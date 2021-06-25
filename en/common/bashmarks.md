---
layout: default
title: "bashmarks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bashmarks">
  <a href="/en/common/bashmarks.html">bashmarks</a> <a href="#bashmarks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Save and jump to commonly used directories using 1 character commands.
> More information: <https://github.com/huyng/bashmarks>.

#### List available bookmarks:
```shell
l
```
#### Save the current directory as "bookmark_name":
```shell
s {{bookmark_name}}
```
#### Go to a bookmarked directory:
```shell
g {{bookmark_name}}
```
#### Print a bookmarked directory's contents:
```shell
p {{bookmark_name}}
```
#### Delete a bookmark:
```shell
d {{bookmark_name}}
```
{% endraw %}