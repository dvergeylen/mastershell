---
layout: default
title: "tmutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tmutil">
  <a href="/en/osx/tmutil.html">tmutil</a> <a href="#tmutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility for managing Time Machine backups. Most verbs require root privileges.
> More information: <https://ss64.com/osx/tmutil.html>.

#### Set a HFS+ drive as the backup destination:
```shell
sudo tmutil setdestination {{path/to/disk_mount_point}}
```
#### Set a APF share or SMB share as the backup destination:
```shell
sudo tmutil setdestination {{protocol://user[:password]@host/share}}
```
#### Append the given destination to the list of destinations:
```shell
sudo tmutil setdestination -a {{destination}}
```
#### Enable automatic backups:
```shell
sudo tmutil enable
```
#### Disable automatic backups:
```shell
sudo tmutil disable
```
#### Start a backup, if one is not running already, and release control of the shell:
```shell
sudo tmutil startbackup
```
#### Start a backup and block until the backup is finished:
```shell
sudo tmutil startbackup -b
```
#### Stop a backup:
```shell
sudo tmutil stopbackup
```
{% endraw %}