---
layout: default
title: "run-mailcap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="run-mailcap">
  <a href="/en/linux/run-mailcap.html">run-mailcap</a> <a href="#run-mailcap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run MailCap Programs.
> Run mailcap view, see, edit, compose, print - execute programs via entries in the mailcap file (or any of its aliases) will use the given action to process each mime-type/file.

#### Individual actions/programs on run-mailcap can be invoked with action flag:
```shell
run-mailcap --action=ACTION [--option[=value]]
```
#### In simple language:
```shell
run-mailcap --action=ACTION {{filename}}
```
#### Turn on extra information:
```shell
run-mailcap --action=ACTION --debug {{filename}}
```
#### Ignore any "copiousoutput" directive and forward output to standard output:
```shell
run-mailcap --action=ACTION --nopager {{filename}}
```
#### Display the found command without actually executing it:
```shell
run-mailcap --action=ACTION --norun {{filename}}
```
{% endraw %}