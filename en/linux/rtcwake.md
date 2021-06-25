---
layout: default
title: "rtcwake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rtcwake">
  <a href="/en/linux/rtcwake.html">rtcwake</a> <a href="#rtcwake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enter a system sleep state until specified wakeup time relative to your bios clock.

#### Show whether an alarm is set or not:
```shell
sudo rtcwake -m show -v
```
#### Suspend to ram and wakeup after 10 seconds:
```shell
sudo rtcwake -m mem -s {{10}}
```
#### Suspend to disk (higher power saving) and wakeup 15 minutes later:
```shell
sudo rtcwake -m disk --date +{{15}}min
```
#### Freeze the system (more efficient than suspend-to-ram but linux > 3.9 required) and wakeup at a given date and time:
```shell
sudo rtcwake -m freeze --date {{YYYYMMDDhhmm}}
```
#### Disable a previously set alarm:
```shell
sudo rtcwake -m disable
```
#### Perform a dry run to wakeup the computer at a given time. (Press Ctrl + C to abort):
```shell
sudo rtcwake -m on --date {{hh:ss}}
```
{% endraw %}