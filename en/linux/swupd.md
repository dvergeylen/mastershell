---
layout: default
title: "swupd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="swupd">
  <a href="/en/linux/swupd.html">swupd</a> <a href="#swupd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package management utility for Clear Linux.
> More information: <https://docs.01.org/clearlinux/latest/guides/clear/swupd.html>.

#### Update to latest version:
```shell
sudo swupd update
```
#### Show current version, and check whether a newer one exists:
```shell
swupd check-update
```
#### List installed bundles:
```shell
swupd bundle-list
```
#### Locate the bundle where a wanted package exists:
```shell
swupd search -b {{package}}
```
#### Install a new bundle:
```shell
sudo swupd bundle-add {{bundle}}
```
#### Remove a bundle:
```shell
sudo swupd bundle-remove {{bundle}}
```
#### Correct broken or missing files:
```shell
sudo swupd verify
```
{% endraw %}