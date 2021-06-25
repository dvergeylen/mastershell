---
layout: default
title: "gpupdate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpupdate">
  <a href="/en/windows/gpupdate.html">gpupdate</a> <a href="#gpupdate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to check and apply Windows Group Policy settings.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/gpupdate>.

#### Check and apply updated Group Policy settings:
```shell
gpupdate
```
#### Specify the target Group Policy settings to check for update:
```shell
gpupdate /target=:{{computer|user}}
```
#### Force all Group Policy settings to be reapplied:
```shell
gpupdate /force
```
#### Display detailed usage information:
```shell
gpupdate /?
```
{% endraw %}