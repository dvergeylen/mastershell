---
layout: default
title: "trash-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="trash-cli">
  <a href="/en/common/trash-cli.html">trash-cli</a> <a href="#trash-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line interface to the trashcan APIs.
> More information: <https://github.com/andreafrancia/trash-cli>.

#### Trash files and directories:
```shell
trash-put {{filename}}
```
#### Empty the trashcan:
```shell
trash-empty
```
#### List trashed files:
```shell
trash-list
```
#### Restore a trashed file by choosing a number from the list that results from this command:
```shell
trash-restore
```
#### Remove individual files from the trashcan:
```shell
trash-rm {{filename}}
```
{% endraw %}