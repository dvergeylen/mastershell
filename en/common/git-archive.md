---
layout: default
title: "git archive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-archive">
  <a href="/en/common/git-archive.html">git archive</a> <a href="#git-archive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create an archive of files from a named tree.
> More information: <https://git-scm.com/docs/git-archive>.

#### Create a tar archive from the contents of the current HEAD and print it to standard output:
```shell
git archive --verbose HEAD
```
#### Create a zip archive from the current HEAD and print it to standard output:
```shell
git archive --verbose --format=zip HEAD
```
#### Same as above, but write the zip archive to file:
```shell
git archive --verbose --output={{path/to/file.zip}} HEAD
```
#### Create a tar archive from the contents of the latest commit on a specific branch:
```shell
git archive --output={{path/to/file.tar}} {{branch_name}}
```
#### Create a tar archive from the contents of a specific directory:
```shell
git archive --output={{path/to/file.tar}} HEAD:{{path/to/directory}}
```
#### Prepend a path to each file to archive it inside a specific directory:
```shell
git archive --output={{path/to/file.tar}} --prefix={{path/to/prepend}}/ HEAD
```
{% endraw %}