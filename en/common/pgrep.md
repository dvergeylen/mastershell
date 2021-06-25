---
layout: default
title: "pgrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pgrep">
  <a href="/en/common/pgrep.html">pgrep</a> <a href="#pgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find or signal processes by name.
> More information: <https://www.man7.org/linux/man-pages/man1/pkill.1.html>.

#### Return PIDs of any running processes with a matching command string:
```shell
pgrep {{process_name}}
```
#### Search for processes including their command-line options:
```shell
pgrep --full "{{process_name}} {{parameter}}"
```
#### Search for processes run by a specific user:
```shell
pgrep --euid root {{process_name}}
```
{% endraw %}