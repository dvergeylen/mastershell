---
layout: default
title: "ipfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipfs">
  <a href="/en/common/ipfs.html">ipfs</a> <a href="#ipfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inter Planetary File System.
> A peer-to-peer hypermedia protocol. Aims to make the web more open.
> More information: <https://ipfs.io>.

#### Add a file from local to the filesystem, pin it and print the relative hash:
```shell
ipfs add {{filename}}
```
#### Add a directory and its files recursively from local to the filesystem and print the relative hash:
```shell
ipfs add -r {{directory}}
```
#### Save a remote file and give it a name but not pin it:
```shell
ipfs get {{hash}} -o {{filename}}
```
#### Pin a remote file locally:
```shell
ipfs pin add {{hash}}
```
#### Display pinned files:
```shell
ipfs pin ls
```
#### Unpin a file from the local storage:
```shell
ipfs pin rm {{hash}}
```
#### Remove unpinned files from local storage:
```shell
ipfs repo gc
```
{% endraw %}