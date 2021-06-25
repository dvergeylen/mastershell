---
layout: default
title: "xargs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xargs">
  <a href="/en/common/xargs.html">xargs</a> <a href="#xargs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute a command with piped arguments coming from another command, a file, etc.
> The input is treated as a single block of text and split into separate pieces on spaces, tabs, newlines and end-of-file.

#### Run a command using the input data as arguments:
```shell
{{arguments_source}} | xargs {{command}}
```
#### Run multiple chained commands on the input data:
```shell
{{arguments_source}} | xargs sh -c "{{command1}} && {{command2}} | {{command3}}"
```
#### Delete all files with a `.backup` extension (`-print0` uses a null character to split file names, and `-0` uses it as delimiter):
```shell
find . -name {{'*.backup'}} -print0 | xargs -0 rm -v
```
#### Execute the command once for each input line, replacing any occurrences of the placeholder (here marked as `_`) with the input line:
```shell
{{arguments_source}} | xargs -I _ {{command}} _ {{optional_extra_arguments}}
```
#### Parallel runs of up to `max-procs` processes at a time; the default is 1. If `max-procs` is 0, xargs will run as many processes as possible at a time:
```shell
{{arguments_source}} | xargs -P {{max-procs}} {{command}}
```
{% endraw %}