---
layout: default
title: "cpufreq-aperf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpufreq-aperf">
  <a href="/en/linux/cpufreq-aperf.html">cpufreq-aperf</a> <a href="#cpufreq-aperf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate the average CPU frequency over a time period.
> Requires root privileges.

#### Start calculating, defaulting to all CPU cores and 1 second refresh interval:
```shell
sudo cpufreq-aperf
```
#### Start calculating for CPU 1 only:
```shell
sudo cpufreq-aperf -c {{1}}
```
#### Start calculating with a 3 seconds refresh interval for all CPU cores:
```shell
sudo cpufreq-aperf -i {{3}}
```
#### Calculate only once:
```shell
sudo cpufreq-aperf -o
```
{% endraw %}