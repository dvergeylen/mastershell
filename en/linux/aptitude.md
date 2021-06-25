---
layout: default
title: "aptitude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aptitude">
  <a href="/en/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian and Ubuntu package management utility.
> More information: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Synchronize list of packages and versions available. This should be run first, before running subsequent aptitude commands:
```shell
aptitude update
```
#### Install a new package and its dependencies:
```shell
aptitude install {{package}}
```
#### Search for a package:
```shell
aptitude search {{package}}
```
#### Search for an installed package (`?installed` is an aptitude search term):
```shell
aptitude search '?installed({{package}})'
```
#### Remove a package and all packages depending on it:
```shell
aptitude remove {{package}}
```
#### Upgrade installed packages to newest available versions:
```shell
aptitude upgrade
```
#### Upgrade installed packages (like `aptitude upgrade`) including removing obsolete packages and installing additional packages to meet new package dependencies:
```shell
aptitude full-upgrade
```
#### Put an installed package on hold to prevent it from being automatically upgraded:
```shell
aptitude hold '?installed({{package}})'
```
{% endraw %}