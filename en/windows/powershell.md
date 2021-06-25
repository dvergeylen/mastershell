---
layout: default
title: "powershell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="powershell">
  <a href="/en/windows/powershell.html">powershell</a> <a href="#powershell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line shell and scripting language designed especially for system administration.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/powershell>.

#### Start a Windows PowerShell session in a Command Prompt window:
```shell
powershell
```
#### Load a specific PowerShell console file:
```shell
powershell -PSConsoleFile {{path/to/file}}
```
#### Start a session with a specified version of PowerShell:
```shell
powershell -Version {{version}}
```
#### Prevent the shell from exit after running startup commands:
```shell
powershell -NoExit
```
#### Describe the format of data sent to PowerShell:
```shell
powershell -InputFormat {{Text|XML}}
```
#### Determine how output from PowerShell is formatted:
```shell
powershell -OutputFormat {{Text|XML}}
```
#### Display help:
```shell
powershell -Help
```
{% endraw %}