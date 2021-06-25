---
layout: default
title: "pacman-mirrors"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman-mirrors">
  <a href="/en/linux/pacman-mirrors.html">pacman-mirrors</a> <a href="#pacman-mirrors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a pacman mirrorlist for Manjaro Linux.
> Every run of pacman-mirrors requires you to synchronize your database and update your system using `sudo pacman -Syyu`.
> More information: <https://wiki.manjaro.org/index.php?title=Pacman-mirrors>.

#### Generate a mirrorlist using the default settings:
```shell
sudo pacman-mirrors --fasttrack
```
#### Get the status of the current mirrors:
```shell
pacman-mirrors --status
```
#### Display the current branch:
```shell
pacman-mirrors --get-branch
```
#### Switch to a different branch:
```shell
sudo pacman-mirrors --api --set-branch {{stable|unstable|testing}}
```
#### Generate a mirrorlist, only using mirrors in your country:
```shell
sudo pacman-mirrors --geoip
```
{% endraw %}