---
layout: default
title: "spi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="spi">
  <a href="/en/linux/spi.html">spi</a> <a href="#spi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A meta package manager that handles both packages and slackbuilds.
> More information: <https://github.com/gapan/spi>.

#### Update the list of available packages and slackbuilds:
```shell
spi --update
```
#### Install a package or slackbuild:
```shell
spi --install {{package/slackbuild_name}}
```
#### Upgrade all installed packages to the latest versions available:
```shell
spi --upgrade
```
#### Locate packages or slackbuilds of interest by package name or description:
```shell
spi {{search_terms}}
```
#### Display information about a package or slackbuild:
```shell
spi --show {{package/slackbuild_name}}
```
#### Purge the local package and slackbuild caches:
```shell
spi --clean
```
{% endraw %}