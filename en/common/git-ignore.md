---
layout: default
title: "git ignore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ignore">
  <a href="/en/common/git-ignore.html">git ignore</a> <a href="#git-ignore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show/update `.gitignore` files.
> Part of `git-extras`. See also `git ignore-io`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-ignore>.

#### Show the content of all global and local `.gitignore` files:
```shell
git ignore
```
#### Ignore file(s) privately, updating `.git/info/exclude` file:
```shell
git ignore {{file_pattern}} --private
```
#### Ignore file(s) locally, updating local `.gitignore` file:
```shell
git ignore {{file_pattern}}
```
#### Ignore file(s) globally, updating global `.gitignore` file:
```shell
git ignore {{file_pattern}} --global
```
{% endraw %}