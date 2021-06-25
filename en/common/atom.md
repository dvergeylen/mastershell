---
layout: default
title: "atom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atom">
  <a href="/en/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A cross-platform pluggable text editor.
> Plugins are managed by `apm`.
> More information: <https://atom.io/>.

#### Open a file or directory:
```shell
atom {{path/to/file_or_directory}}
```
#### Open a file or directory in a new window:
```shell
atom -n {{path/to/file_or_directory}}
```
#### Open a file or directory in an existing window:
```shell
atom --add {{path/to/file_or_directory}}
```
#### Open Atom in safe mode (does not load any additional packages):
```shell
atom --safe
```
#### Prevent Atom from forking into the background, keeping Atom attached to the terminal:
```shell
atom --foreground
```
#### Wait for Atom window to close before returning (useful for Git commit editor):
```shell
atom --wait
```
{% endraw %}