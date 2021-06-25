---
layout: default
title: "rename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rename">
  <a href="/en/linux/file-rename.html">rename</a> <a href="#rename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename multiple files.
> NOTE: this page refers to the command from the `file-rename` Debian package.

#### Rename files using a Perl Common Regular Expression (substitute 'foo' with 'bar' wherever found):
```shell
rename {{'s/foo/bar/'}} {{*}}
```
#### Dry-run - display which renames would occur without performing them:
```shell
rename -n {{'s/foo/bar/'}} {{*}}
```
#### Force renaming even if the operation would remove existing destination files:
```shell
rename -f {{'s/foo/bar/'}} {{*}}
```
#### Convert filenames to lower case (use `-f` in case-insensitive filesystems to prevent "already exists" errors):
```shell
rename 'y/A-Z/a-z/' {{*}}
```
#### Replace whitespace with underscores:
```shell
rename 's/\s+/_/g' {{*}}
```
{% endraw %}