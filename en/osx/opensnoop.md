---
layout: default
title: "opensnoop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="opensnoop">
  <a href="/en/osx/opensnoop.html">opensnoop</a> <a href="#opensnoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool that tracks file opens on your system.

#### Print all file opens as they occur:
```shell
sudo opensnoop
```
#### Track all file opens by a process by name:
```shell
sudo opensnoop -n {{process_name}}
```
#### Track all file opens by a process by PID:
```shell
sudo opensnoop -p {{PID}}
```
#### Track which processes open a specified file:
```shell
sudo opensnoop -f {{path/to/file}}
```
{% endraw %}