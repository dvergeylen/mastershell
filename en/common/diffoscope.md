---
layout: default
title: "diffoscope"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="diffoscope">
  <a href="/en/common/diffoscope.html">diffoscope</a> <a href="#diffoscope"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare files, archives, and directories.
> More information: <https://diffoscope.org>.

#### Compare two files:
```shell
diffoscope {{path/to/file1}} {{path/to/file2}}
```
#### Compare two files without displaying a progress bar:
```shell
diffoscope --no-progress {{path/to/file1}} {{path/to/file2}}
```
#### Compare two files and write a HTML-report to a file (use `-` for stdout):
```shell
diffoscope --html {{path/to/outfile|-}} {{path/to/file1}} {{path/to/file2}}
```
#### Compare two directories excluding files with a name matching a specified pattern:
```shell
diffoscope --exclude {{pattern}} {{path/to/directory1}} {{path/to/directory2}}
```
#### Compare two directories and control whether directory metadata is considered:
```shell
diffoscope --exclude-directory-metadata {{auto|yes|no|recursive}} {{path/to/directory1}} {{path/to/directory2}}
```
{% endraw %}