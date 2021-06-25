---
layout: default
title: "stow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stow">
  <a href="/en/common/stow.html">stow</a> <a href="#stow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Symlink manager.
> Often used to manage dotfiles.
> More information: <https://www.gnu.org/software/stow>.

#### Symlink all files recursively to a given directory:
```shell
stow --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}
```
#### Delete symlinks recursively from a given directory:
```shell
stow --delete --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}
```
#### Simulate to see what the result would be like:
```shell
stow --simulate --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}
```
#### Delete and resymlink:
```shell
stow --restow --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}
```
#### Exclude files matching a regular expression:
```shell
stow --ignore={{regular_expression}} --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}
```
{% endraw %}