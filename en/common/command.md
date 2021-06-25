---
layout: default
title: "command"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="command">
  <a href="/en/common/command.html">command</a> <a href="#command"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command forces the shell to execute the program and ignore any functions, builtins and aliases with the same name.
> More information: <https://manned.org/command>.

#### Execute the `ls` program literally, even if an `ls` alias exists:
```shell
command {{ls}}
```
#### Display the path to the executable or the alias definition of a specific command:
```shell
command -v {{command_name}}
```
{% endraw %}