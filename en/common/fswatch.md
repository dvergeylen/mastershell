---
layout: default
title: "fswatch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fswatch">
  <a href="/en/common/fswatch.html">fswatch</a> <a href="#fswatch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A cross-platform file change monitor.
> More information: <https://emcrisostomo.github.io/fswatch>.

#### Run a bash command on file creation, update or deletion:
```shell
fswatch {{path/to/file}} | xargs -n 1 {{bash_command}}
```
#### Watch one or more files and/or directories:
```shell
fswatch {{path/to/file}} {{path/to/directory}} {{path/to/another_directory/**/*.js}} | xargs -n 1 {{bash_command}}
```
#### Print the absolute paths of the changed files:
```shell
fswatch {{path/to/directory}} | xargs -n 1 -I {} echo {}
```
#### Filter by event type, eg. Updated, Deleted or Created:
```shell
fswatch --event {{Updated}} {{path/to/directory}} | xargs -n 1 {{bash_command}}
```
{% endraw %}