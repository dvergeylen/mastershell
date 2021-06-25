---
layout: default
title: "tar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tar">
  <a href="/en/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Archiving utility.
> Often combined with a compression method, such as gzip or bzip2.
> More information: <https://www.gnu.org/software/tar>.

#### [c]reate an archive and write it to a [f]ile:
```shell
tar cf {{target.tar}} {{file1}} {{file2}} {{file3}}
```
#### [c]reate a g[z]ipped archive and write it to a [f]ile:
```shell
tar czf {{target.tar.gz}} {{file1}} {{file2}} {{file3}}
```
#### [c]reate a g[z]ipped archive from a directory using relative paths:
```shell
tar czf {{target.tar.gz}} --directory={{path/to/directory}} .
```
#### E[x]tract a (compressed) archive [f]ile into the current directory [v]erbosely:
```shell
tar xvf {{source.tar[.gz|.bz2|.xz]}}
```
#### E[x]tract a (compressed) archive [f]ile into the target directory:
```shell
tar xf {{source.tar[.gz|.bz2|.xz]}} --directory={{directory}}
```
#### [c]reate a compressed archive and write it to a [f]ile, using [a]rchive suffix to determine the compression program:
```shell
tar caf {{target.tar.xz}} {{file1}} {{file2}} {{file3}}
```
#### Lis[t] the contents of a tar [f]ile [v]erbosely:
```shell
tar tvf {{source.tar}}
```
#### E[x]tract files matching a pattern from an archive [f]ile:
```shell
tar xf {{source.tar}} --wildcards "{{*.html}}"
```
{% endraw %}