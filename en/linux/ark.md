---
layout: default
title: "ark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ark">
  <a href="/en/linux/ark.html">ark</a> <a href="#ark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KDE archiving tool.
> More information: <https://docs.kde.org/stable5/en/kdeutils/ark/>.

#### Extract an archive into the current directory:
```shell
ark --batch {{archive}}
```
#### Change extraction directory:
```shell
ark --batch --destination {{path/to/directory}} {{archive}}
```
#### Create an archive if it does not exist and add files to it:
```shell
ark --add-to {{archive}} {{file1}} {{file2}}
```
{% endraw %}