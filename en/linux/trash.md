---
layout: default
title: "trash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="trash">
  <a href="/en/linux/trash.html">trash</a> <a href="#trash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI for managing your trashcan / recycling bin.
> More information: <https://github.com/andreafrancia/trash-cli>.

#### Delete a file (send to trash):
```shell
trash {{path/to/file}}
```
#### List files in trash:
```shell
trash-list
```
#### Restore file from trash:
```shell
trash-restore
```
#### Empty trash:
```shell
trash-empty
```
#### Empty trash, keeping files trashed less than {{10}} days ago:
```shell
trash-empty {{10}}
```
#### Remove all files named 'foo' from the trash:
```shell
trash-rm foo
```
#### Remove all files with a given original location:
```shell
trash-rm {{/absolute/path/to/file_or_directory}}
```
{% endraw %}