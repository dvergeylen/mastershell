---
layout: default
title: "softwareupdate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="softwareupdate">
  <a href="/en/osx/softwareupdate.html">softwareupdate</a> <a href="#softwareupdate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for updating macOS App Store apps via the command-line.

#### List all available updates:
```shell
softwareupdate -l
```
#### Download and install all updates:
```shell
softwareupdate -ia
```
#### Download and install all recommended updates:
```shell
softwareupdate -ir
```
#### Download and install a specific app:
```shell
softwareupdate -i {{update_name}}
```
{% endraw %}