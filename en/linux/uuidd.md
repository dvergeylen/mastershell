---
layout: default
title: "uuidd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uuidd">
  <a href="/en/linux/uuidd.html">uuidd</a> <a href="#uuidd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Daemon for generating UUIDs.
> More information: <https://manned.org/uuidd>.

#### Generate a random UUID:
```shell
uuidd --random
```
#### Generate a bulk number of random UUIDs:
```shell
uuidd --random --uuids {{number_of_uuids}}
```
#### Generate a time-based UUID, based on the current time and MAC address of the system:
```shell
uuidd --time
```
{% endraw %}