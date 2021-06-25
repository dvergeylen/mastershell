---
layout: default
title: "fsck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fsck">
  <a href="/en/osx/fsck.html">fsck</a> <a href="#fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check the integrity of a filesystem or repair it. The filesystem should be unmounted at the time the command is run.
> It is a wrapper that calls `fsck_hfs`, `fsck_apfs`, `fsck_msdos`, `fsck_exfat`, and `fsck_udf` as needed.

#### Check filesystem `/dev/sdX`, reporting any damaged blocks:
```shell
fsck {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX` only if it is clean, reporting any damaged blocks and interactively letting the user choose to repair each one:
```shell
fsck -f {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX` only if it is clean, reporting any damaged blocks and automatically repairing them:
```shell
fsck -fy {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX`, reporting whether it has been cleanly unmounted:
```shell
fsck -q {{/dev/sdX}}
```
{% endraw %}