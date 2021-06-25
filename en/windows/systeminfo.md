---
layout: default
title: "systeminfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="systeminfo">
  <a href="/en/windows/systeminfo.html">systeminfo</a> <a href="#systeminfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display operating system configuration for a local or remote machine.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/systeminfo>.

#### Display system configuration for the local machine:
```shell
systeminfo
```
#### Display system configuration in a specified output format:
```shell
systeminfo /fo {{table|list|csv}}
```
#### Display system configuration for a remote machine:
```shell
systeminfo /s {{remote_name}} /u {{username}} /p {{password}}
```
#### Display detailed usage information:
```shell
systeminfo /?
```
{% endraw %}