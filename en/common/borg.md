---
layout: default
title: "borg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="borg">
  <a href="/en/common/borg.html">borg</a> <a href="#borg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deduplicating backup tool.
> Creates local or remote backups that are mountable as filesystems.
> More information: <https://borgbackup.readthedocs.io/en/stable/usage/general.html>.

#### Initialise a (local) repository:
```shell
borg init {{path/to/repo_directory}}
```
#### Backup a directory into the repository, creating an archive called "Monday":
```shell
borg create --progress {{path/to/repo_directory}}::{{Monday}} {{path/to/source_directory}}
```
#### List all archives in a repository:
```shell
borg list {{path/to/repo_directory}}
```
#### Extract a specific directory from the "Monday" archive in a remote repository, excluding all `*.ext` files:
```shell
borg extract {{user}}@{{host}}:{{path/to/repo_directory}}::{{Monday}} {{path/to/target_directory}} --exclude '{{*.ext}}'
```
#### Prune a repository by deleting all archives older than 7 days, listing changes:
```shell
borg prune --keep-within {{7d}} --list {{path/to/repo_directory}}
```
#### Mount a repository as a FUSE filesystem:
```shell
borg mount {{path/to/repo_directory}}::{{Monday}} {{path/to/mountpoint}}
```
#### Display help on creating archives:
```shell
borg create --help
```
{% endraw %}