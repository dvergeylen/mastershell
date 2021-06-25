---
layout: default
title: "lynis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lynis">
  <a href="/en/linux/lynis.html">lynis</a> <a href="#lynis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> System and security auditing tool.
> More information: <https://cisofy.com/documentation/lynis/>.

#### Check that Lynis is up-to-date:
```shell
sudo lynis update info
```
#### Run a security audit of the system:
```shell
sudo lynis audit system
```
#### Run a security audit of a Dockerfile:
```shell
sudo lynis audit dockerfile {{path/to/dockerfile}}
```
{% endraw %}