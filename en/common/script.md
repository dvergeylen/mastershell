---
layout: default
title: "script"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="script">
  <a href="/en/common/script.html">script</a> <a href="#script"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Make a typescript file of a terminal session.

#### Start recording in file named "typescript":
```shell
script
```
#### Stop recording:
```shell
exit
```
#### Start recording in a given file:
```shell
script {{logfile.log}}
```
#### Append to an existing file:
```shell
script -a {{logfile.log}}
```
#### Execute quietly without start and done messages:
```shell
script -q {{logfile.log}}
```
{% endraw %}