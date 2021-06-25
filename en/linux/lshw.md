---
layout: default
title: "lshw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lshw">
  <a href="/en/linux/lshw.html">lshw</a> <a href="#lshw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List detailed information about hardware configurations as root user.

#### Launch the GUI:
```shell
sudo lshw -X
```
#### List all hardwares in tabular format:
```shell
sudo lshw -short
```
#### List all disks and storage controllers in tabular format:
```shell
sudo lshw -class disk -class storage -short
```
#### Save all network interfaces to an HTML file:
```shell
sudo lshw -class network -html > {{interfaces.html}}
```
{% endraw %}