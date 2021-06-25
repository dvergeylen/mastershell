---
layout: default
title: "zoxide"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zoxide">
  <a href="/en/common/zoxide.html">zoxide</a> <a href="#zoxide"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Keep track of the most frequently used directories.
> Uses a ranking algorithm to navigate to the best match.
> More information: <https://github.com/ajeetdsouza/zoxide>.

#### Go to the highest-ranked directory that contains "foo" in the name:
```shell
zoxide query {{foo}}
```
#### Go to the highest-ranked directory that contains "foo" and then "bar":
```shell
zoxide query {{foo}} {{bar}}
```
#### Start an interactive directory search (requires `fzf`):
```shell
zoxide query --interactive
```
#### Add a directory or increment its rank:
```shell
zoxide add {{path/to/directory}}
```
#### Remove a directory from `zoxide`'s database:
```shell
zoxide remove {{path/to/directory}}
```
#### Generate shell configuration for command aliases (`z`, `za`, `zi`, `zq`, `zr`):
```shell
zoxide init {{bash|fish|zsh}}
```
{% endraw %}