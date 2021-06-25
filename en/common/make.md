---
layout: default
title: "make"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="make">
  <a href="/en/common/make.html">make</a> <a href="#make"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Task runner for targets described in Makefile.
> Mostly used to control the compilation of an executable from source code.
> More information: <https://www.gnu.org/software/make/manual/make.html>.

#### Call the first target specified in the Makefile (usually named "all"):
```shell
make
```
#### Call a specific target:
```shell
make {{target}}
```
#### Call a specific target, executing 4 jobs at a time in parallel:
```shell
make -j{{4}} {{target}}
```
#### Use a specific Makefile:
```shell
make --file {{file}}
```
#### Execute make from another directory:
```shell
make --directory {{directory}}
```
#### Force making of a target, even if source files are unchanged:
```shell
make --always-make {{target}}
```
#### Override variables defined in the Makefile by the environment:
```shell
make --environment-overrides {{target}}
```
{% endraw %}