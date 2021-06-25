---
layout: default
title: "delta"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="delta">
  <a href="/en/common/delta.html">delta</a> <a href="#delta"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A viewer for Git and diff output.
> More information: <https://github.com/dandavison/delta>.

#### Compare files or directories:
```shell
delta {{path/to/old_file_or_directory}} {{path/to/new_file_or_directory}}
```
#### Compare files or directories, showing the line numbers:
```shell
delta --line-numbers {{path/to/old_file_or_directory}} {{path/to/new_file_or_directory}}
```
#### Compare files or directories, showing the differences side by side:
```shell
delta --side-by-side {{path/to/old_file_or_directory}} {{path/to/new_file_or_directory}}
```
#### Compare files or directories, ignoring any Git configuration settings:
```shell
delta --no-gitconfig {{path/to/old_file_or_directory}} {{path/to/new_file_or_directory}}
```
#### Compare, rendering commit hashes, file names, and line numbers as hyperlinks, according to the hyperlink spec for terminal emulators:
```shell
delta --hyperlinks {{path/to/old_file_or_directory}} {{path/to/new_file_or_directory}}
```
#### Display the current settings:
```shell
delta --show-config
```
#### Display supported languages and associated file extensions:
```shell
delta --list-languages
```
{% endraw %}