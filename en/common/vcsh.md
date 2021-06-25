---
layout: default
title: "vcsh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vcsh">
  <a href="/en/common/vcsh.html">vcsh</a> <a href="#vcsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Version Control System for the home directory using Git repositories.
> More information: <https://github.com/RichiH/vcsh>.

#### Initialize an (empty) repository:
```shell
vcsh init {{repository_name}}
```
#### Clone a repository into a custom directory name:
```shell
vcsh clone {{git_url}} {{repository_name}}
```
#### List all managed repositories:
```shell
vcsh list
```
#### Execute a Git command on a managed repository:
```shell
vcsh {{repository_name}} {{git_command}}
```
#### Push/pull all managed repositories to/from remotes:
```shell
vcsh {{push|pull}}
```
#### Write a custom `.gitignore` file for a managed repository:
```shell
vcsh write-gitignore {{repository_name}}
```
{% endraw %}