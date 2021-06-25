---
layout: default
title: "hdparm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hdparm">
  <a href="/en/linux/hdparm.html">hdparm</a> <a href="#hdparm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get and set SATA and IDE hard drive parameters.

#### Request the identification info of a given device:
```shell
sudo hdparm -I /dev/{{device}}
```
#### Get the Advanced Power Management level:
```shell
sudo hdparm -B /dev/{{device}}
```
#### Set the Advanced Power Management value (values 1-127 permit spin-down, and values 128-254 do not):
```shell
sudo hdparm -B {{1}} /dev/{{device}}
```
#### Display the device's current power mode status:
```shell
sudo hdparm -C /dev/{{device}}
```
#### Force a drive to immediately enter standby mode (usually causes a drive to spin down):
```shell
sudo hdparm -y /dev/{{device}}
```
#### Put the drive into idle (low-power) mode, also setting its standby timeout:
```shell
sudo hdparm -S {{standby_timeout}} {{device}}
```
{% endraw %}