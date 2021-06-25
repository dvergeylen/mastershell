---
layout: default
title: "iscc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iscc">
  <a href="/en/windows/iscc.html">iscc</a> <a href="#iscc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compiler for Inno Setup installers.
> It compiles an Inno Setup scripts into an Windows installer executable.
> More information: <https://jrsoftware.org/isinfo.php>.

#### Compile an Inno Setup script:
```shell
iscc {{path/to/file.iss}}
```
#### Quietly compile an Inno Setup installer:
```shell
iscc /Q {{path/to/file.iss}}
```
#### Compile a signed Inno Setup installer:
```shell
iscc /S={{name}}={{command}} {{path/to/file.iss}}
```
{% endraw %}