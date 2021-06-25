---
layout: default
title: "finger"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="finger">
  <a href="/en/windows/finger.html">finger</a> <a href="#finger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Return information about one or more users on a specified system.
> The remote system must be running the Finger service.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/finger>.

#### Display information about a specific user:
```shell
finger {{user}}@{{host}}
```
#### Display information about all users on the specified host:
```shell
finger @{{host}}
```
#### Display information in a longer format:
```shell
finger {{user}}@{{host}} -l
```
#### Display help information:
```shell
finger /?
```
{% endraw %}