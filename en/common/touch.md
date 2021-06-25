---
layout: default
title: "touch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="touch">
  <a href="/en/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change a file access and modification times (atime, mtime).
> More information: <https://www.gnu.org/software/coreutils/touch>.

#### Create a new empty file(s) or change the times for existing file(s) to current time:
```shell
touch {{filename}}
```
#### Set the times on a file to a specific date and time:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{filename}}
```
#### Use the times from a file to set the times on a second file:
```shell
touch -r {{filename}} {{filename2}}
```
#### Create multiple files:
```shell
touch {{file{1,2,3}.txt}}
```
{% endraw %}