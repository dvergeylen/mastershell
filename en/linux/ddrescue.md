---
layout: default
title: "ddrescue"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ddrescue">
  <a href="/en/linux/ddrescue.html">ddrescue</a> <a href="#ddrescue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Data recovery tool that reads data from damaged block devices.
> More information: <https://www.gnu.org/software/ddrescue/>.

#### Take an image of a device, creating a log file:
```shell
sudo ddrescue {{/dev/sdb}} {{path/to/image.dd}} {{path/to/log.txt}}
```
#### Clone Disk A to Disk B, creating a log file:
```shell
sudo ddrescue --force --no-scrape {{/dev/sdX}} {{/dev/sdY}} {{path/to/log.txt}}
```
{% endraw %}