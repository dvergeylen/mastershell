---
layout: default
title: "cpio"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpio">
  <a href="/en/common/cpio.html">cpio</a> <a href="#cpio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copies files in and out of archives.
> Supports the following archive formats: cpio's custom binary, old ASCII, new ASCII, crc, HPUX binary, HPUX old ASCII, old tar, and POSIX.1 tar.
> More information: <https://www.gnu.org/software/cpio>.

#### Take a list of file names from standard input and add them [o]nto an archive in cpio's binary format:
```shell
echo "{{file1}} {{file2}} {{file3}}" | cpio -o > {{archive.cpio}}
```
#### Copy all files and directories in a directory and add them [o]nto an archive, in [v]erbose mode:
```shell
find {{path/to/directory}} | cpio -ov > {{archive.cpio}}
```
#### P[i]ck all files from an archive, generating [d]irectories where needed, in [v]erbose mode:
```shell
cpio -idv < {{archive.cpio}}
```
{% endraw %}