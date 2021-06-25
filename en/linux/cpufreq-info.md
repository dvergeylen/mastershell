---
layout: default
title: "cpufreq-info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpufreq-info">
  <a href="/en/linux/cpufreq-info.html">cpufreq-info</a> <a href="#cpufreq-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to show CPU frequency information.

#### Show CPU frequency information for all CPUs:
```shell
cpufreq-info
```
#### Show CPU frequency information for the specified CPU:
```shell
cpufreq-info -c {{cpu_number}}
```
#### Show the allowed minimum and maximum CPU frequency:
```shell
cpufreq-info -l
```
#### Show the current minimum and maximum CPU frequency and policy in table format:
```shell
cpufreq-info -o
```
#### Show available CPU frequency policies:
```shell
cpufreq-info -g
```
#### Show current CPU work frequency in a human-readable format, according to the cpufreq kernel module:
```shell
cpufreq-info -f -m
```
#### Show current CPU work frequency in a human-readable format, by reading it from hardware (only available to root):
```shell
sudo cpufreq-info -w -m
```
{% endraw %}