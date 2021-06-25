---
layout: default
title: "restic"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="restic">
  <a href="/en/common/restic.html">restic</a> <a href="#restic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A backup program that aims to be fast, secure and efficient.
> More information: <https://restic.net>.

#### Initialize a backup repository in the specified local directory:
```shell
restic init -r {{path/to/repository}}
```
#### Backup a directory to the repository:
```shell
restic -r {{path/to/repository}} backup {{path/to/directory}}
```
#### Show backup snapshots currently stored in the repository:
```shell
restic -r {{path/to/repository}} snapshots
```
#### Restore a specific backup snapshot to a target directory:
```shell
restic -r {{path/to/repository}} restore {{snapshot_id}} {{path/to/target}}
```
#### Restore a specific path from a specific backup to a target directory:
```shell
restic -r {{path/to/repository}} --include {{path/to/restore}} --target {{path/to/target}} restore {{snapshot_id}}
```
#### Clean up the repository and keep only the most recent snapshot of each unique backup:
```shell
restic forget --keep-last 1 --prune
```
{% endraw %}