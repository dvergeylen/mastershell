---
layout: default
title: "rg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rg">
  <a href="/en/common/rg.html">rg</a> <a href="#rg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ripgrep is a recursive line-oriented CLI search tool.
> Aims to be a faster alternative to `grep`.
> More information: <https://github.com/BurntSushi/ripgrep>.

#### Recursively search the current directory for a regular expression:
```shell
rg {{regular_expression}}
```
#### Search for regular expressions recursively in the current directory, including hidden files and files listed in `.gitignore`:
```shell
rg --no-ignore --hidden {{regular_expression}}
```
#### Search for a regular expression only in a certain filetype (e.g., html, css, etc.):
```shell
rg --type {{filetype}} {{regular_expression}}
```
#### Search for a regular expression only in a subset of directories:
```shell
rg {{regular_expression}} {{set_of_subdirs}}
```
#### Search for a regular expression in files matching a glob (e.g., `README.*`):
```shell
rg {{regular_expression}} --glob {{glob}}
```
#### Only list matched files (useful when piping to other commands):
```shell
rg --files-with-matches {{regular_expression}}
```
#### Show lines that do not match the given regular expression:
```shell
rg --invert-match {{regular_expression}}
```
#### Search a literal string pattern:
```shell
rg --fixed-strings -- {{string}}
```
{% endraw %}