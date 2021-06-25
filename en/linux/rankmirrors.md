---
layout: default
title: "rankmirrors"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rankmirrors">
  <a href="/en/linux/rankmirrors.html">rankmirrors</a> <a href="#rankmirrors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rank a list of Pacman mirrors by connection and opening speed.
> Writes the new mirrorlist to stdout.
> More information: <https://wiki.archlinux.org/index.php/mirrors>.

#### Rank a mirror list:
```shell
rankmirrors {{/etc/pacman.d/mirrorlist}}
```
#### Output only a given number of the top ranking servers:
```shell
rankmirrors -n {{number}} {{/etc/pacman.d/mirrorlist}}
```
#### Be verbose when generating the mirrorlist:
```shell
rankmirrors -v {{/etc/pacman.d/mirrorlist}}
```
#### Test only a specific URL:
```shell
rankmirrors --url {{url}}
```
#### Output only the response times instead of a full mirrorlist:
```shell
rankmirrors --times {{/etc/pacman.d/mirrorlist}}
```
{% endraw %}