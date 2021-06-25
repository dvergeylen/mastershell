---
layout: default
title: "ed"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ed">
  <a href="/en/common/ed.html">ed</a> <a href="#ed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The original Unix text editor.
> More information: <https://man.archlinux.org/man/ed.1>.

#### Start ed, editing an empty document (which can be saved as a new file in the current directory):
```shell
ed
```
#### Start ed, editing an empty document, with `:` as a command prompt indicator:
```shell
ed -p :
```
#### Start ed editing an existing file (this shows the byte count of the loaded file):
```shell
ed -p : {{path/to/file}}
```
#### Toggle the printing of error explanations. (By default, explanations are not printed and only a `?` appears):
```shell
H
```
#### Add text to the current document. Mark completion by entering a period by itself in a new line:
```shell
a<Enter>{{text_to_insert}}<Enter>.
```
#### Print the entire document (`,` is a shortcut to the range `1,$` which covers the start to the end of the document):
```shell
,p
```
#### Write the current document to a new file (the filename can be omitted if `ed` was called with an existing file):
```shell
w {{filename}}
```
#### Quit ed:
```shell
q
```
{% endraw %}