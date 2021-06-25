---
layout: default
title: "reg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg">
  <a href="/en/windows/reg.html">reg</a> <a href="#reg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line interface for managing keys and their values in the Windows registry.
> See `reg-query`, `reg-add` and other pages for additional information.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg>.

#### Execute registry commands:
```shell
reg {{command}}
```
#### Display general information and list all available commands:
```shell
reg /?
```
#### Call help on a specific command:
```shell
reg {{command}} /?
```
{% endraw %}