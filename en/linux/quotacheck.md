---
layout: default
title: "quotacheck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="quotacheck">
  <a href="/en/linux/quotacheck.html">quotacheck</a> <a href="#quotacheck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scan a filesystem for disk usage; create, check and repair quota files.
> It is best to run quota check with quotas turned off to prevent damage or loss to quota files.

#### Check quotas on all mounted non-NFS filesystems:
```shell
sudo quotacheck --all
```
#### Force check even if quotas are enabled (this can cause damage or loss to quota files):
```shell
sudo quotacheck --force {{mountpoint}}
```
#### Check quotas on a given filesystem in debug mode:
```shell
sudo quotacheck --debug {{mountpoint}}
```
#### Check quotas on a given filesystem, displaying the progress:
```shell
sudo quotacheck --verbose {{mountpoint}}
```
#### Check user quotas:
```shell
sudo quotacheck --user {{user}} {{mountpoint}}
```
#### Check group quotas:
```shell
sudo quotacheck --group {{group}} {{mountpoint}}
```
{% endraw %}