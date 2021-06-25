---
layout: default
title: "calibredb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="calibredb">
  <a href="/en/common/calibredb.html">calibredb</a> <a href="#calibredb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to manipulate the your e-book database.
> Part of the Calibre e-book library.
> More information: <https://manual.calibre-ebook.com/generated/en/calibredb.html>.

#### List e-books in the library with additional information:
```shell
calibredb list
```
#### Search for e-books displaying additional information:
```shell
calibredb list --search {{search_term}}
```
#### Search for just ids of e-books:
```shell
calibredb search {{search_term}}
```
#### Add one or more e-books to the library:
```shell
calibredb add {{file1 file2 …}}
```
#### Recursively add all e-books under a directory to the library:
```shell
calibredb add -r {{path/to/directory}}
```
#### Remove one or more e-books from the library. You need the e-book IDs (see above):
```shell
calibredb remove {{id1 id2 …}}
```
{% endraw %}