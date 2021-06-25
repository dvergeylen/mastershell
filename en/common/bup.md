---
layout: default
title: "bup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bup">
  <a href="/en/common/bup.html">bup</a> <a href="#bup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Backup system based on the Git packfile format, providing incremental saves and global deduplication.
> More information: <https://github.com/bup/bup>.

#### Initialize a backup repository in the specified local directory:
```shell
bup -d {{path/to/repository}} init
```
#### Prepare a given directory before taking a backup:
```shell
bup -d {{path/to/repository}} index {{path/to/directory}}
```
#### Backup a directory to the repository:
```shell
bup -d {{path/to/repository}} save -n {{backup_name}} {{path/to/directory}}
```
#### Show the backup snapshots currently stored in the repository:
```shell
bup -d {{path/to/repository}} ls
```
#### Restore a specific backup snapshot to a target directory:
```shell
bup -d {{path/to/repository}} restore -C {{path/to/target_directory}} {{backup_name}}
```
{% endraw %}