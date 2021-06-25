---
layout: default
title: "expect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="expect">
  <a href="/en/linux/expect.html">expect</a> <a href="#expect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Script executor that interacts with other programs that require user input.
> More information: <https://manned.org/expect>.

#### Execute an expect script from a file:
```shell
expect {{path/to/file}}
```
#### Execute a specified expect script:
```shell
expect -c "{{commands}}"
```
#### Enter an interactive REPL (use `exit` or Ctrl + D to exit):
```shell
expect -i
```
{% endraw %}