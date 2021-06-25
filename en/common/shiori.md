---
layout: default
title: "shiori"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shiori">
  <a href="/en/common/shiori.html">shiori</a> <a href="#shiori"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple bookmark manager built with Go.
> More information: <https://github.com/go-shiori/shiori>.

#### Import bookmarks from HTML Netscape bookmark format file:
```shell
shiori import {{path/to/bookmarks.html}}
```
#### Save the specified URL as bookmark:
```shell
shiori add {{url}}
```
#### List the saved bookmarks:
```shell
shiori print
```
#### Open the saved bookmark in a browser:
```shell
shiori open {{bookmark_id}}
```
#### Start the web interface for managing bookmarks at port 8181:
```shell
shiori serve --port {{8181}}
```
{% endraw %}