---
layout: default
title: "rename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rename">
  <a href="/en/linux/rename.html">rename</a> <a href="#rename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename multiple files.
> NOTE: this page refers to the command from the `util-linux` package.
> For the Perl version, see `file-rename` or `perl-rename`.
> Warning: This command has no safeguards and will overwrite files without prompting.

#### Rename files using simple substitutions (substitute 'foo' with 'bar' wherever found):
```shell
rename {{foo}} {{bar}} {{*}}
```
#### Dry-run - display which renames would occur without performing them:
```shell
rename -vn {{foo}} {{bar}} {{*}}
```
#### Do not overwrite existing files:
```shell
rename -o {{foo}} {{bar}} {{*}}
```
#### Change file extensions:
```shell
rename {{.ext}} {{.bak}} {{*.ext}}
```
#### Prepend "foo" to all filenames in the current directory:
```shell
rename {{''}} {{'foo'}} {{*}}
```
#### Rename a group of increasingly numbered files zero-padding the numbers up to 3 digits:
```shell
rename {{foo}} {{foo00}} {{foo?}} && rename {{foo}} {{foo0}} {{foo??}}
```
{% endraw %}