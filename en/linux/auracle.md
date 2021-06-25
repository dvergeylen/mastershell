---
layout: default
title: "auracle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="auracle">
  <a href="/en/linux/auracle.html">auracle</a> <a href="#auracle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool used to interact with Arch Linux's User Repository, commonly referred to as the AUR.
> More information: <https://github.com/falconindy/auracle>.

#### Display AUR packages that match a regular expression:
```shell
auracle search '{{regular_expression}}'
```
#### Display package information for a space-separated list of AUR packages:
```shell
auracle info {{package1}} {{package2}}
```
#### Display the `PKGBUILD` file (build information) for a space-separated list of AUR packages:
```shell
auracle show {{package1}} {{package2}}
```
#### Display updates for installed AUR packages:
```shell
auracle outdated
```
{% endraw %}