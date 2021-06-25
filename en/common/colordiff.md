---
layout: default
title: "colordiff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="colordiff">
  <a href="/en/common/colordiff.html">colordiff</a> <a href="#colordiff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to colorize diff output.
> The Perl script colordiff is a wrapper for `diff` and produces the same output but with pretty syntax highlighting. Colour schemes can be customized.
> More information: <https://github.com/kimmel/colordiff>.

#### Compare files:
```shell
colordiff {{file1}} {{file2}}
```
#### Output in two columns:
```shell
colordiff -y {{file1}} {{file2}}
```
#### Ignore case differences in file contents:
```shell
colordiff -i {{file1}} {{file2}}
```
#### Report when two files are the same:
```shell
colordiff -s {{file1}} {{file2}}
```
#### Ignore white spaces:
```shell
colordiff -w {{file1}} {{file2}}
```
{% endraw %}