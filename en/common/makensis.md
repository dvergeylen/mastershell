---
layout: default
title: "makensis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="makensis">
  <a href="/en/common/makensis.html">makensis</a> <a href="#makensis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cross-platform compiler for NSIS installers.
> It compiles a NSIS script into a Windows installer executable.
> More information: <https://nsis.sourceforge.io/Docs/Chapter3.html>.

#### Compile a NSIS script:
```shell
makensis {{path/to/file.nsi}}
```
#### Compile a NSIS script in strict mode (treat warnings as errors):
```shell
makensis -WX {{path/to/file.nsi}}
```
#### Print help for a specific command:
```shell
makensis -CMDHELP {{command}}
```
{% endraw %}