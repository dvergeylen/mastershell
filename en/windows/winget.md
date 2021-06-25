---
layout: default
title: "winget"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="winget">
  <a href="/en/windows/winget.html">winget</a> <a href="#winget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows Package Manager CLI.
> More information: <https://docs.microsoft.com/windows/package-manager/winget>.

#### Install a package:
```shell
winget install {{package}}
```
#### Display information about a package:
```shell
winget show {{package}}
```
#### Search for a package:
```shell
winget search {{package}}
```
{% endraw %}