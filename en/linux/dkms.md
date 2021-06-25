---
layout: default
title: "dkms"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dkms">
  <a href="/en/linux/dkms.html">dkms</a> <a href="#dkms"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A framework that allows for dynamic building of kernel modules.
> More information: <https://github.com/dell/dkms>.

#### List currently installed modules:
```shell
dkms status
```
#### Rebuild all modules for the currently running kernel:
```shell
dkms autoinstall
```
#### Install version 1.2.1 of the acpi_call module for the currently running kernel:
```shell
dkms install -m {{acpi_call}} -v {{1.2.1}}
```
#### Remove version 1.2.1 of the acpi_call module from all kernels:
```shell
dkms remove -m {{acpi_call}} -v {{1.2.1}} --all
```
{% endraw %}