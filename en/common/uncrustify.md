---
layout: default
title: "uncrustify"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uncrustify">
  <a href="/en/common/uncrustify.html">uncrustify</a> <a href="#uncrustify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> C, C++, C#, D, Java and Pawn source code formatter.
> More information: <https://github.com/uncrustify/uncrustify>.

#### Format a single file:
```shell
uncrustify -f {{path/to/file.cpp}} -o {{path/to/output.cpp}}
```
#### Read filenames from stdin, and take backups before writing output back to the original filepaths:
```shell
find . -name "*.cpp" | uncrustify -F - --replace
```
#### Don't make backups (useful if files are under version control):
```shell
find . -name "*.cpp" | uncrustify -F - --no-backup
```
#### Use a custom configuration file and write the result to stdout:
```shell
uncrustify -c {{path/to/uncrustify.cfg}} -f {{path/to/file.cpp}}
```
#### Explicitly set a configuration variable's value:
```shell
uncrustify --set {{option}}={{value}}
```
#### Generate a new configuration file:
```shell
uncrustify --update-config -o {{path/to/new.cfg}}
```
{% endraw %}