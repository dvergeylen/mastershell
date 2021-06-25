---
layout: default
title: "exec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exec">
  <a href="/en/common/exec.html">exec</a> <a href="#exec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Replace the current process with another process.

#### Replace with the specified command using the current environment variables:
```shell
exec {{command -with -flags}}
```
#### Replace with the specified command, clearing environment variables:
```shell
exec -c {{command -with -flags}}
```
#### Replace with the specified command and login using the default shell:
```shell
exec -l {{command -with -flags}}
```
#### Replace with the specified command and change the process name:
```shell
exec -a {{process_name}} {{command -with -flags}}
```
{% endraw %}