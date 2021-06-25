---
layout: default
title: "mdls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mdls">
  <a href="/en/osx/mdls.html">mdls</a> <a href="#mdls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the metadata attributes for a file.

#### Display the list of metadata attributes for file:
```shell
mdls {{path/to/file}}
```
#### Display a specific metadata attribute:
```shell
mdls -name {{attribute}} {{path/to/file}}
```
{% endraw %}