---
layout: default
title: "powertop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="powertop">
  <a href="/en/linux/powertop.html">powertop</a> <a href="#powertop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Optimize battery power usage.

#### Calibrate power usage measurements:
```shell
sudo powertop --calibrate
```
#### Generate HTML power usage report in the current directory:
```shell
sudo powertop --html={{power_report.html}}
```
#### Tune to optimal settings:
```shell
sudo powertop --auto-tune
```
{% endraw %}