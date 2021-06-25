---
layout: default
title: "okular"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="okular">
  <a href="/en/common/okular.html">okular</a> <a href="#okular"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A universal document viewer.
> More information: <https://okular.kde.org/>.

#### Launch Okular:
```shell
okular
```
#### Open specific documents in Okular:
```shell
okular {{path/to/file1 path/to/file2 ...}}
```
#### Open a document at a specific page:
```shell
okular --page {{page_number}} {{path/to/file}}
```
#### Open a document in presentation mode:
```shell
okular --presentation {{path/to/file}}
```
#### Open a document and start the print dialog:
```shell
okular --print {{path/to/file}}
```
#### Open a document and search for a specific string:
```shell
okular --find {{search_string}} {{path/to/file}}
```
{% endraw %}