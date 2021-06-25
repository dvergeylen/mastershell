---
layout: default
title: "acpi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="acpi">
  <a href="/en/linux/acpi.html">acpi</a> <a href="#acpi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shows battery status or thermal information.
> More information: <https://sourceforge.net/projects/acpiclient/files/acpiclient/>.

#### Show battery information:
```shell
acpi
```
#### Show thermal information:
```shell
acpi -t
```
#### Show cooling device information:
```shell
acpi -c
```
#### Show thermal information in Fahrenheit:
```shell
acpi -tf
```
#### Show all information:
```shell
acpi -V
```
#### Extract information from `/proc` instead of `/sys`:
```shell
acpi -p
```
{% endraw %}