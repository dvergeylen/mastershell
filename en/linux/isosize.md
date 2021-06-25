---
layout: default
title: "isosize"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="isosize">
  <a href="/en/linux/isosize.html">isosize</a> <a href="#isosize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the size of an ISO file.
> More information: <https://manned.org/isosize>.

#### Display the size of an ISO file:
```shell
isosize {{path/to/file.iso}}
```
#### Display the block count and block size of an ISO file:
```shell
isosize --sectors {{path/to/file.iso}}
```
#### Display the size of an ISO file divided by a given number (only usable when --sectors is not given):
```shell
isosize --divisor={{number}} {{path/to/file.iso}}
```
{% endraw %}