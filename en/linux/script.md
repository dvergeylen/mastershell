---
layout: default
title: "script"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="script">
  <a href="/en/linux/script.html">script</a> <a href="#script"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Record all terminal output to file.

#### Record a new session to a file named `typescript` in the current directory:
```shell
script
```
#### Record a new session to a custom filepath:
```shell
script {{path/to/session.out}}
```
#### Record a new session, appending to an existing file:
```shell
script -a {{path/to/session.out}}
```
#### Record timing information (data is outputted to the standard error):
```shell
script -t 2> {{path/to/timingfile}}
```
{% endraw %}