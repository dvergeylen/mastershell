---
layout: default
title: "system_profiler"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="system_profiler">
  <a href="/en/osx/system_profiler.html">system_profiler</a> <a href="#system_profiler"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report system hardware and software configuration.

#### Display a full system profiler report which can be opened by System Profiler.app:
```shell
system_profiler -xml > MyReport.spx
```
#### Display a hardware overview (Model, CPU, Memory, Serial, etc):
```shell
system_profiler SPHardwareDataType
```
#### Print the system serial number:
```shell
system_profiler SPHardwareDataType|grep "Serial Number (system)" |awk '{print $4}'
```
{% endraw %}