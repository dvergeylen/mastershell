---
layout: default
title: "chkdsk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chkdsk">
  <a href="/en/windows/chkdsk.html">chkdsk</a> <a href="#chkdsk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check file system and volume metadata for errors.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/chkdsk>.

#### Specify the drive letter (followed by a colon), mount point, or volume name to check:
```shell
chkdsk {{volume}}
```
#### Fix errors on a specific volume:
```shell
chkdsk {{volume}} /f
```
#### Dismount a specific volume before checking:
```shell
chkdsk {{volume}} /x
```
#### Change the log file size to the specified size (only for NTFS):
```shell
chkdsk /l{{size}}
```
{% endraw %}