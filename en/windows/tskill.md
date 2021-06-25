---
layout: default
title: "tskill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tskill">
  <a href="/en/windows/tskill.html">tskill</a> <a href="#tskill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ends a process running in a session on a Remote Desktop Session Host.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/tskill>.

#### Terminate a process by its process identifier:
```shell
tskill {{process_id}}
```
#### Terminate a process by its name:
```shell
tskill {{process_name}}
```
{% endraw %}