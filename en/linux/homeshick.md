---
layout: default
title: "homeshick"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="homeshick">
  <a href="/en/linux/homeshick.html">homeshick</a> <a href="#homeshick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Synchronize Git dotfiles.
> More information: <https://github.com/andsens/homeshick/wiki>.

#### Create a new castle:
```shell
homeshick generate {{castle_name}}
```
#### Add a file to your castle:
```shell
homeshick track {{castle_name}} {{path/to/file}}
```
#### Go to a castle:
```shell
homeshick cd {{castle_name}}
```
#### Clone a castle:
```shell
homeshick clone {{github_username}}/{{repository_name}}
```
#### Symlink all files from a castle:
```shell
homeshick link {{castle_name}}
```
{% endraw %}