---
layout: default
title: "rsync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rsync">
  <a href="/en/common/rsync.html">rsync</a> <a href="#rsync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transfer files either to or from a remote host (not between two remote hosts).
> Can transfer single files, or multiple files matching a pattern.

#### Transfer file from local to remote host:
```shell
rsync {{path/to/local_file}} {{remote_host}}:{{path/to/remote_directory}}
```
#### Transfer file from remote host to local:
```shell
rsync {{remote_host}}:{{path/to/remote_file}} {{path/to/local_directory}}
```
#### Transfer file in [a]rchive (to preserve attributes) and compressed ([z]ipped) mode with [v]erbose and [h]uman-readable [P]rogress:
```shell
rsync -azvhP {{path/to/local_file}} {{remote_host}}:{{path/to/remote_directory}}
```
#### Transfer a directory and all its children from a remote to local:
```shell
rsync -r {{remote_host}}:{{path/to/remote_directory}} {{path/to/local_directory}}
```
#### Transfer directory contents (but not the directory itself) from a remote to local:
```shell
rsync -r {{remote_host}}:{{path/to/remote_directory}}/ {{path/to/local_directory}}
```
#### Transfer a directory [r]ecursively, in [a]rchive to preserve attributes, resolving contained soft[l]inks , and ignoring already transferred files [u]nless newer:
```shell
rsync -rauL {{remote_host}}:{{path/to/remote_file}} {{path/to/local_directory}}
```
#### Transfer file over SSH and delete local files that do not exist on remote host:
```shell
rsync -e ssh --delete {{remote_host}}:{{path/to/remote_file}} {{path/to/local_file}}
```
#### Transfer file over SSH using a different port than the default and show global progress:
```shell
rsync -e 'ssh -p {{port}}' --info=progress2 {{remote_host}}:{{path/to/remote_file}} {{path/to/local_file}}
```
{% endraw %}