---
layout: default
title: "sh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sh">
  <a href="/en/common/sh.html">sh</a> <a href="#sh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne shell, the standard command language interpreter.
> See also `histexpand` for history expansion.
> More information: <https://manned.org/sh>.

#### Start an interactive shell session:
```shell
sh
```
#### Execute a command and then exit:
```shell
sh -c "{{command}}"
```
#### Execute a script:
```shell
sh {{path/to/script.sh}}
```
#### Read and execute commands from stdin:
```shell
sh -s
```
{% endraw %}