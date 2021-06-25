---
layout: default
title: "f3fix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="f3fix">
  <a href="/en/common/f3fix.html">f3fix</a> <a href="#f3fix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Edit the partition table of a fake flash drive.
> See also `f3probe`, `f3write`, `f3read`.
> More information: <http://oss.digirati.com.br/f3/>.

#### Fill a fake flash drive with a single partition that matches its real capacity:
```shell
sudo f3fix {{/dev/device_name}}
```
#### Mark the partition as bootable:
```shell
sudo f3fix --boot {{/dev/device_name}}
```
#### Specify the filesystem:
```shell
sudo f3fix --fs-type={{filesystem_type}} {{/dev/device_name}}
```
{% endraw %}