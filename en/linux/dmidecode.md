---
layout: default
title: "dmidecode"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmidecode">
  <a href="/en/linux/dmidecode.html">dmidecode</a> <a href="#dmidecode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the DMI (alternatively known as SMBIOS) table contents in a human-readable format.
> Requires root privileges.

#### Show all DMI table contents:
```shell
sudo dmidecode
```
#### Show the BIOS version:
```shell
sudo dmidecode -s bios-version
```
#### Show the system's serial number:
```shell
sudo dmidecode -s system-serial-number
```
#### Show BIOS information:
```shell
sudo dmidecode -t bios
```
#### Show CPU information:
```shell
sudo dmidecode -t processor
```
#### Show memory information:
```shell
sudo dmidecode -t memory
```
{% endraw %}