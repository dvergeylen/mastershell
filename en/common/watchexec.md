---
layout: default
title: "watchexec"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="watchexec">
  <a href="/en/common/watchexec.html">watchexec</a> <a href="#watchexec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run arbitrary commands when files change.
> More information: <https://github.com/watchexec/watchexec>.

#### Call `ls -la` when any file in the current directory changes:
```shell
watchexec -- {{ls -la}}
```
#### Run `make` when any JavaScript, CSS and HTML files in the current directory change:
```shell
watchexec --exts {{js,css,html}} make
```
#### Run `make` when any file in the `lib` or `src` subdirectories change:
```shell
watchexec --watch {{lib}} --watch {{src}} {{make}}
```
#### Call/restart `my_server` when any file in the current directory change, sending `SIGKILL` to stop the child process:
```shell
watchexec --restart --signal {{SIGKILL}} {{my_server}}
```
{% endraw %}