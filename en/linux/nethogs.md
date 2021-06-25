---
layout: default
title: "nethogs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nethogs">
  <a href="/en/linux/nethogs.html">nethogs</a> <a href="#nethogs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor bandwidth usage per process.
> More information: <https://github.com/raboof/nethogs>.

#### Start nethogs as root (default device is eth0):
```shell
sudo nethogs
```
#### Monitor bandwidth on specific device:
```shell
sudo nethogs {{device}}
```
#### Monitor bandwidth on multiple devices:
```shell
sudo nethogs {{device1}} {{device2}}
```
#### Specify refresh rate:
```shell
sudo nethogs -t {{seconds}}
```
{% endraw %}