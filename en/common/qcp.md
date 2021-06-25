---
layout: default
title: "qcp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qcp">
  <a href="/en/common/qcp.html">qcp</a> <a href="#qcp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files using the default text editor to define the filenames.
> More information: <https://www.nongnu.org/renameutils/>.

#### Copy a single file (open an editor with the source filename on the left and the target filename on the right):
```shell
qcp {{source_file}}
```
#### Copy multiple JPG files:
```shell
qcp {{*.jpg}}
```
#### Copy files, but swap the positions of the source and the target filenames in the editor:
```shell
qcp --option swap {{*.jpg}}
```
{% endraw %}