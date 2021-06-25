---
layout: default
title: "extundelete"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="extundelete">
  <a href="/en/linux/extundelete.html">extundelete</a> <a href="#extundelete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recover deleted files from ext3 or ext4 partitions by parsing the journal.
> See also `date` for Unix time information and `umount` for unmounting partitions.
> More information: <http://extundelete.sourceforge.net>.

#### Restore all deleted files inside partition N on device X:
```shell
sudo extundelete {{/dev/sdXN}} --restore-all
```
#### Restore a file from a path relative to root (Do not start the path with `/`):
```shell
extundelete {{/dev/sdXN}} --restore-file {{path/to/file}}
```
#### Restore a directory from a path relative to root (Do not start the path with `/`):
```shell
extundelete {{/dev/sdXN}} --restore-directory {{path/to/directory}}
```
#### Restore all files deleted after January 1st, 2020 (in Unix time):
```shell
extundelete {{/dev/sdXN}} --restore-all --after {{1577840400}}
```
{% endraw %}