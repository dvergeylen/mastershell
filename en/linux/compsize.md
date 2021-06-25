---
layout: default
title: "compsize"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="compsize">
  <a href="/en/linux/compsize.html">compsize</a> <a href="#compsize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate the compression ratio of a set of files on a btrfs filesystem.
> See also `btrfs filesystem` for recompressing a file by defragmenting it.
> More information: <https://github.com/kilobyte/compsize>.

#### Calculate the current compression ratio for a file or directory:
```shell
sudo compsize {{path/to/file_or_directory}}
```
#### Don't traverse filesystem boundaries:
```shell
sudo compsize --one-file-system {{path/to/file_or_directory}}
```
#### Show raw byte counts instead of human-readable sizes:
```shell
sudo compsize --bytes {{path/to/file_or_directory}}
```
{% endraw %}