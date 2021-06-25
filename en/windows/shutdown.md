---
layout: default
title: "shutdown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shutdown">
  <a href="/en/windows/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for shutting down, restarting or logging off a machine.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/shutdown>.

#### Shutdown the current machine:
```shell
shutdown /s
```
#### Shutdown the current machine force-closing all apps:
```shell
shutdown /s /f
```
#### Restart the current machine immediately:
```shell
shutdown /r /t 0
```
#### Hibernate the current machine:
```shell
shutdown /h
```
#### Log off the current machine:
```shell
shutdown /l
```
#### Specify a timeout in seconds to wait before shutting down:
```shell
shutdown /s /t {{seconds}}
```
#### Abort a shutdown sequence whose timeout is yet to expire:
```shell
shutdown /a
```
#### Shutdown a remote machine:
```shell
shutdown /m {{\\hostname}}
```
{% endraw %}