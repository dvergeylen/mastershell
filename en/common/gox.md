---
layout: default
title: "gox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gox">
  <a href="/en/common/gox.html">gox</a> <a href="#gox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for cross-compiling Go programs.
> More information: <https://github.com/mitchellh/gox>.

#### Compile Go program in the current directory for all operating systems and architecture combinations:
```shell
gox
```
#### Download and compile a Go program from a remote URL:
```shell
gox {{url_1}} {{url_2}}
```
#### Compile current directory for a particular operating system:
```shell
gox -os="{{os}}"
```
#### Compile current directory for a single operating system and architecture combination:
```shell
gox -osarch="{{os}}/{{arch}}"
```
{% endraw %}