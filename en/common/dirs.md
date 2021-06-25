---
layout: default
title: "dirs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirs">
  <a href="/en/common/dirs.html">dirs</a> <a href="#dirs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays or manipulates the directory stack.
> The directory stack is a list of recently visited directories that can be manipulated with the `pushd` and `popd` commands.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#Directory-Stack-Builtins>.

#### Display the directory stack with a space between each entry:
```shell
dirs
```
#### Display the directory stack with one entry per line:
```shell
dirs -p
```
#### Display only the nth entry in the directory stack, starting at 0:
```shell
dirs +{{N}}
```
#### Clear the directory stack:
```shell
dirs -c
```
{% endraw %}