---
layout: default
title: "buku"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="buku">
  <a href="/en/common/buku.html">buku</a> <a href="#buku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line browser-independent bookmark manager.
> More information: <https://github.com/jarun/Buku>.

#### Display all bookmarks matching "keyword" and with "privacy" tag:
```shell
buku {{keyword}} --stag {{privacy}}
```
#### Add bookmark with tags "search engine" and "privacy":
```shell
buku --add {{https://example.com}} {{search engine}}, {{privacy}}
```
#### Delete a bookmark:
```shell
buku --delete {{bookmark_id}}
```
#### Open editor to edit a bookmark:
```shell
buku --write {{bookmark_id}}
```
#### Remove "search engine" tag from a bookmark:
```shell
buku --update {{bookmark_id}} --tag {{-}} {{search engine}}
```
{% endraw %}