---
layout: default
title: "tlp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tlp">
  <a href="/en/linux/tlp.html">tlp</a> <a href="#tlp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Advanced power management for Linux.
> See also `tlp-stat`.
> More information: <https://linrunner.de/tlp/>.

#### Apply settings (according to the actual power source):
```shell
sudo tlp start
```
#### Apply battery settings (ignoring the actual power source):
```shell
sudo tlp bat
```
#### Apply AC settings (ignoring the actual power source):
```shell
sudo tlp ac
```
{% endraw %}