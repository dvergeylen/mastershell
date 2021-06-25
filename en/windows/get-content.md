---
layout: default
title: "Get-Content"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="get-content">
  <a href="/en/windows/get-content.html">Get-Content</a> <a href="#get-content"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get the content of the item at the specified location.
> More information: <https://docs.microsoft.com/powershell/module/microsoft.powershell.management/get-content>.

#### Display the content of a file:
```shell
Get-Content -Path {{path/to/file}}
```
#### Display the first few lines of a file:
```shell
Get-Content -Path {{path/to/file}} -TotalCount {{count}}
```
#### Display the content of the file and keep reading from it until `Ctrl + C` is pressed:
```shell
Get-Content -Path {{path/to/file}} -Wait
```
{% endraw %}