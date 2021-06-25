---
layout: default
title: "whence"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whence">
  <a href="/en/osx/whence.html">whence</a> <a href="#whence"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A zsh builtin to indicate how a given command would be interpreted.

#### Interpret {{command}}, with expansion if defined as an `alias` (similar to the `command -v` builtin):
```shell
whence {{command}}
```
#### Display type of {{command}}, with location if defined as a function, or binary (equivalent to the `type` and `command -V` builtins):
```shell
whence -v {{command}}
```
#### Same as above, except display content of shell functions instead of location (equivalent to `which` builtin):
```shell
whence -c {{command}}
```
#### Same as above, but show all occurrences on command path (equivalent to the `where` builtin):
```shell
whence -ca {{command}}
```
#### Search only the `PATH` for {{command}}, ignoring builtins, aliases or shell functions (equivalent to the `where` command):
```shell
whence -p {{command}}
```
{% endraw %}