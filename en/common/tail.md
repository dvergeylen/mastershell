---
layout: default
title: "tail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tail">
  <a href="/en/common/tail.html">tail</a> <a href="#tail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the last part of a file.
> More information: <https://www.gnu.org/software/coreutils/tail>.

#### Show last 'num' lines in file:
```shell
tail -n {{num}} {{file}}
```
#### Show all file since line 'num':
```shell
tail -n +{{num}} {{file}}
```
#### Show last 'num' bytes in file:
```shell
tail -c {{num}} {{file}}
```
#### Keep reading file until `Ctrl + C`:
```shell
tail -f {{file}}
```
#### Keep reading file until `Ctrl + C`, even if the file is rotated:
```shell
tail -F {{file}}
```
#### Show last 'num' lines in 'file' and refresh every 'n' seconds:
```shell
tail -n {{num}} -s {{n}} -f {{file}}
```
{% endraw %}