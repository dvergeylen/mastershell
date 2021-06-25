---
layout: default
title: "cpufreq-set"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpufreq-set">
  <a href="/en/linux/cpufreq-set.html">cpufreq-set</a> <a href="#cpufreq-set"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to modify CPU frequency settings.
> The frequency value should range between the output of command `cpufreq-info -l`.

#### Set the CPU frequency policy of CPU 1 to "userspace":
```shell
sudo cpufreq-set -c {{1}} -g {{userspace}}
```
#### Set the current minimum CPU frequency of CPU 1:
```shell
sudo cpufreq-set -c {{1}} --min {{min_frequency}}
```
#### Set the current maximum CPU frequency of CPU 1:
```shell
sudo cpufreq-set -c {{1}} --max {{max_frequency}}
```
#### Set the current work frequency of CPU 1:
```shell
sudo cpufreq-set -c {{1}} -f {{work_frequency}}
```
{% endraw %}