---
layout: default
title: "balooctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="balooctl">
  <a href="/en/linux/balooctl.html">balooctl</a> <a href="#balooctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> File indexing and searching framework for KDE Plasma.
> More information: <https://wiki.archlinux.org/index.php/Baloo>.

#### Display help:
```shell
balooctl
```
#### Display the status of the indexer:
```shell
balooctl status
```
#### Enable/Disable the file indexer:
```shell
balooctl {{enable|disable}}
```
#### Clean the index database:
```shell
balooctl purge
```
#### Suspend the file indexer:
```shell
balooctl suspend
```
#### Resume the file indexer:
```shell
balooctl resume
```
#### Display the disk space used by Baloo:
```shell
balooctl indexSize
```
#### Check for any unindexed files and index them:
```shell
balooctl check
```
{% endraw %}