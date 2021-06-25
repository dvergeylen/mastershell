---
layout: default
title: "duperemove"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="duperemove">
  <a href="/en/linux/duperemove.html">duperemove</a> <a href="#duperemove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Finds duplicate filesystem extents and optionally schedule them for deduplication.
> An extent is small part of a file inside the filesystem.
> On some filesystems one extent can be referenced multiple times, when parts of the content of the files are identical.
> More information: <https://markfasheh.github.io/duperemove/>.

#### Search for duplicate extents in a directory and show them:
```shell
duperemove -r {{path/to/directory}}
```
#### Deduplicate duplicate extents on a Btrfs or XFS (experimental) filesystem:
```shell
duperemove -r -d {{path/to/directory}}
```
#### Use a hash file to store extent hashes (less memory usage and can be reused on subsequent runs):
```shell
duperemove -r -d --hashfile={{path/to/hashfile}} {{path/to/directory}}
```
#### Limit I/O threads (for hashing and dedupe stage) and CPU threads (for duplicate extent finding stage):
```shell
duperemove -r -d --hashfile={{path/to/hashfile}} --io-threads={{N}} --cpu-threads={{N}} {{path/to/directory}}
```
{% endraw %}