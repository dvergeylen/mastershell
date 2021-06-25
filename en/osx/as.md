---
layout: default
title: "as"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="as">
  <a href="/en/osx/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Portable GNU assembler.
> Primarily intended to assemble output from `gcc` to be used by `ld`.

#### Assemble a file, writing the output to `a.out`:
```shell
as {{file.s}}
```
#### Assemble the output to a given file:
```shell
as {{file.s}} -o {{out.o}}
```
#### Generate output faster by skipping whitespace and comment preprocessing. (Should only be used for trusted compilers):
```shell
as -f {{file.s}}
```
#### Include a given path to the list of directories to search for files specified in `.include` directives:
```shell
as -I {{path/to/directory}} {{file.s}}
```
{% endraw %}