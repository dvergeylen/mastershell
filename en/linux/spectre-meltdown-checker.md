---
layout: default
title: "spectre-meltdown-checker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="spectre-meltdown-checker">
  <a href="/en/linux/spectre-meltdown-checker.html">spectre-meltdown-checker</a> <a href="#spectre-meltdown-checker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Spectre and Meltdown mitigation detection tool.
> More information: <https://manned.org/spectre-meltdown-checker.1>.

#### Check the currently running kernel for Spectre or Meltdown:
```shell
sudo spectre-meltdown-checker
```
#### Check the currently running kernel and show an explanation of the actions to take in order to mitigate a vulnerability:
```shell
sudo spectre-meltdown-checker --explain
```
#### Check for specific variants (defaults to all):
```shell
sudo spectre-meltdown-checker --variant {{1|2|3|3a|4|l1tf|msbds|mfbds|mlpds|mdsum|taa|mcespc|srbds}}
```
#### Display output using a specific output format:
```shell
sudo spectre-meltdown-checker --batch {{text|json|nrpe|prometheus|short}}
```
#### Don't use the `/sys` interface even if present:
```shell
sudo spectre-meltdown-checker --no-sysfs
```
#### Check a non-running kernel:
```shell
sudo spectre-meltdown-checker --kernel {{path/to/kernel_file}}
```
{% endraw %}