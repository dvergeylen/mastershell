---
layout: default
title: "mimetype"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mimetype">
  <a href="/en/linux/mimetype.html">mimetype</a> <a href="#mimetype"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Automatically determine the MIME type of a file.

#### Print the MIME type of a given file:
```shell
mimetype {{path/to/file}}
```
#### Display only the MIME type, and not the filename:
```shell
mimetype --brief {{path/to/file}}
```
#### Display a description of the MIME type:
```shell
mimetype --describe {{path/to/file}}
```
#### Determine the MIME type of stdin (does not check a filename):
```shell
{{some_command}} | mimetype --stdin
```
#### Display debug information about how the MIME type was determined:
```shell
mimetype --debug {{path/to/file}}
```
#### Display all the possible MIME types of a given file in confidence order:
```shell
mimetype --all {{path/to/file}}
```
#### Explicitly specify the 2-letter language code of the output:
```shell
mimetype --language {{path/to/file}}
```
{% endraw %}