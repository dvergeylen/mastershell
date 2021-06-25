---
layout: default
title: "rclone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rclone">
  <a href="/en/common/rclone.html">rclone</a> <a href="#rclone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI program to copy/sync/move files and directories to and from many cloud services.
> More information: <https://rclone.org>.

#### List contents of a directory on an rclone remote:
```shell
rclone lsf {{remote_name}}:{{path/to/directory}}
```
#### Copy file or directory from local source to remote destination:
```shell
rclone copy {{path/to/source_file_or_directory}} {{remote_name}}:{{path/to/destination_directory}}
```
#### Copy file or directory from remote source to local destination:
```shell
rclone copy {{remote_name}}:{{path/to/source_file_or_directory}} {{path/to/destination_directory}}
```
#### Sync local source to remote destination, changing the destination only:
```shell
rclone sync {{path/to/file_or_directory}} {{remote_name}}:{{path/to/directory}}
```
#### Move file or directory from local source to remote destination:
```shell
rclone move {{path/to/file_or_directory}} {{remote_name}}:{{path/to/directory}}
```
#### Delete remote file or directory (use `--dry-run` to test, remove it to actually delete):
```shell
rclone --dry-run delete {{remote_name}}:{{path/to/file_or_directory}}
```
#### Mount rclone remote (experimental):
```shell
rclone mount {{remote_name}}:{{path/to/directory}} {{path/to/mount_point}}
```
#### Unmount rclone remote if CTRL-C fails (experimental):
```shell
fusermount -u {{path/to/mount_point}}
```
{% endraw %}