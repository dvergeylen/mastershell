---
layout: default
title: "git daemon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-daemon">
  <a href="/en/common/git-daemon.html">git daemon</a> <a href="#git-daemon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A really simple server for Git repositories.
> More information: <https://git-scm.com/docs/git-daemon>.

#### Launch a Git daemon with a whitelisted set of directories:
```shell
git daemon --export-all {{path/to/directory1}} {{path/to/directory2}}
```
#### Launch a Git daemon with a specific base directory and allow pulling from all sub-directories that look like Git repositories:
```shell
git daemon --base-path={{path/to/directory}} --export-all --reuseaddr
```
#### Launch a Git daemon for the specified directory, verbosely printing log messages and allowing Git clients to write to it:
```shell
git daemon {{path/to/directory}} --enable=receive-pack --informative-errors --verbose
```
{% endraw %}