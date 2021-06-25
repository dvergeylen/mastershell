---
layout: default
title: "dust"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dust">
  <a href="/en/common/dust.html">dust</a> <a href="#dust"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dust gives an instant overview of which directories are using disk space.
> More information: <https://github.com/bootandy/dust>.

#### Display information for the current directory:
```shell
dust
```
#### Display information for a space-separated list of directories:
```shell
dust {{path/to/directory1}} {{path/to/directory2}}
```
#### Display 30 directories (defaults to 21):
```shell
dust --number-of-lines {{30}}
```
#### Display information for the current directory, up to 3 levels deep:
```shell
dust --depth {{3}}
```
#### Display the biggest directories at the top in descending order:
```shell
dust --reverse
```
#### Ignore all files and directories with a specific name:
```shell
dust --ignore-directory {{file_or_directory_name}}
```
#### Do not display percent bars and percentages:
```shell
dust --no-percent-bars
```
{% endraw %}