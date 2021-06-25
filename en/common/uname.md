---
layout: default
title: "uname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uname">
  <a href="/en/common/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print details about the current machine and the operating system running on it.
> Note: for additional information about the operating system, try the `lsb_release` command.
> More information: <https://www.gnu.org/software/coreutils/uname>.

#### Print hardware-related information: machine and processor:
```shell
uname -mp
```
#### Print software-related information: operating system, release number, and version:
```shell
uname -srv
```
#### Print the nodename (hostname) of the system:
```shell
uname -n
```
#### Print all available system information (hardware, software, nodename):
```shell
uname -a
```
{% endraw %}