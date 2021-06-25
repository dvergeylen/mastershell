---
layout: default
title: "realpath"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="realpath">
  <a href="/en/common/realpath.html">realpath</a> <a href="#realpath"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the resolved absolute path for a file or directory.
> More information: <https://www.gnu.org/software/coreutils/realpath>.

#### Display the absolute path for a file or directory:
```shell
realpath {{path/to/file_or_directory}}
```
#### Require all path components to exist:
```shell
realpath --canonicalize-existing {{path/to/file_or_directory}}
```
#### Resolve ".." components before symlinks:
```shell
realpath --logical {{path/to/file_or_directory}}
```
#### Disable symlink expansion:
```shell
realpath --no-symlinks {{path/to/file_or_directory}}
```
#### Suppress error messages:
```shell
realpath --quiet {{path/to/file_or_directory}}
```
{% endraw %}