---
layout: default
title: "choco pack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-pack">
  <a href="/en/windows/choco-pack.html">choco pack</a> <a href="#choco-pack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package a NuGet specification into a nupkg file.
> More information: <https://chocolatey.org/docs/commands-pack>.

#### Package a NuGet specification to a nupkg file:
```shell
choco pack {{path/to/specification}}
```
#### Package a NuGet specification specifying the version of the resulting file:
```shell
choco pack {{path/to/specification}} --version {{version}}
```
#### Package a NuGet specification to a specific directory:
```shell
choco pack {{path/to/specification}} --output-directory {{path/to/output_directory}}
```
{% endraw %}