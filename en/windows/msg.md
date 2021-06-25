---
layout: default
title: "msg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="msg">
  <a href="/en/windows/msg.html">msg</a> <a href="#msg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send a message to a specific user or session.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/msg>.

#### Send a message to a specified user or session:
```shell
msg {{username|session_name|session_id}} {{message}}
```
#### Send a message from stdin:
```shell
echo "{{message}}" | msg {{username|session_name|session_id}}
```
#### Send a message to a specific server:
```shell
msg /server:{{server_name}} {{username|session_name|session_id}}
```
#### Send a message to all users of the current machine:
```shell
msg *
```
#### Set a delay in seconds for a message:
```shell
msg /time:{{seconds}}
```
{% endraw %}