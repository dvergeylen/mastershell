---
layout: default
title: "git-maintenance"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-maintenance">
  <a href="/en/common/git-maintenance.html">git-maintenance</a> <a href="#git-maintenance"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run tasks to optimize Git repository data.
> More information: <https://git-scm.com/docs/git-maintenance>.

#### Register the current repository in the user's list of repositories to daily have maintenance run:
```shell
git maintenance register
```
#### Start running maintenance on the current repository:
```shell
git maintenance start
```
#### Halt the background maintenance schedule for the current repository:
```shell
git maintenance stop
```
#### Remove the current repository from the user's maintenance repository list:
```shell
git maintenance unregister
```
#### Run a specific maintenance task on the current repository:
```shell
git maintenance run --task={{commit-graph|gc|incremental-repack|loose-objects|pack-refs|prefetch}}
```
{% endraw %}