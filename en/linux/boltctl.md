---
layout: default
title: "boltctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="boltctl">
  <a href="/en/linux/boltctl.html">boltctl</a> <a href="#boltctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control thunderbolt devices.
> More information: <https://manned.org/boltctl>.

#### List connected (and authorized) devices:
```shell
boltctl
```
#### List connected devices, including unauthorized ones:
```shell
boltctl list
```
#### Authorize a device temporarily:
```shell
boltctl authorize {{device_uuid}}
```
#### Authorize and remember a device:
```shell
boltctl enroll {{device_uuid}}
```
#### Revoke a previously authorized device:
```shell
boltctl forget {{device_uuid}}
```
#### Show more information about a device:
```shell
boltctl info {{device_uuid}}
```
{% endraw %}