---
layout: default
title: "logoff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logoff">
  <a href="/en/windows/logoff.html">logoff</a> <a href="#logoff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminate a login session.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/logoff>.

#### Terminate the current session:
```shell
logoff
```
#### Terminate a session by its name or id:
```shell
logoff {{session_name|session_id}}
```
#### Terminate a session on a specific server connected through RDP:
```shell
logoff {{session_name|session_id}} /server:{{servername}}
```
{% endraw %}