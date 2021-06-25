---
layout: default
title: "btrfs scrub"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btrfs-scrub">
  <a href="/en/linux/btrfs-scrub.html">btrfs scrub</a> <a href="#btrfs-scrub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scrub btrfs filesystems to verify data integrity.
> It is recommended to run a scrub once a month.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-scrub>.

#### Start a scrub:
```shell
sudo btrfs scrub start {{path/to/btrfs_mount}}
```
#### Show the status of an ongoing or last completed scrub:
```shell
sudo btrfs scrub status {{path/to/btrfs_mount}}
```
#### Cancel an ongoing scrub:
```shell
sudo btrfs scrub cancel {{path/to/btrfs_mount}}
```
#### Resume a previously cancelled scrub:
```shell
sudo btrfs scrub resume {{path/to/btrfs_mount}}
```
#### Start a scrub, but wait until the scrub finishes before exiting:
```shell
sudo btrfs scrub start -B {{path/to/btrfs_mount}}
```
#### Start a scrub in quiet mode (does not print errors or statistics):
```shell
sudo btrfs scrub start -q {{path/to/btrfs_mount}}
```
{% endraw %}