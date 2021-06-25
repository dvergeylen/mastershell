---
layout: default
title: "apt-mark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-mark">
  <a href="/en/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to change the status of installed packages.
> More information: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Mark a package as automatically installed:
```shell
sudo apt-mark auto {{package_name}}
```
#### Hold a package at its current version and prevent updates to it:
```shell
sudo apt-mark hold {{package_name}}
```
#### Allow a package to be updated again:
```shell
sudo apt-mark unhold {{package_name}}
```
#### Show manually installed packages:
```shell
apt-mark showmanual
```
#### Show held packages that aren't being updated:
```shell
apt-mark showhold
```
{% endraw %}