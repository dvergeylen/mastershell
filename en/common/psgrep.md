---
layout: default
title: "psgrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="psgrep">
  <a href="/en/common/psgrep.html">psgrep</a> <a href="#psgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search running processes with `grep`.
> More information: <https://jvz.github.io/psgrep>.

#### Find process lines containing a specific string:
```shell
psgrep {{process_name}}
```
#### Find process lines containing a specific string, excluding headers:
```shell
psgrep -n {{process_name}}
```
#### Search using a simplified format (PID, user, command):
```shell
psgrep -s {{process_name}}
```
{% endraw %}