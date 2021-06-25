---
layout: default
title: "git notes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-notes">
  <a href="/en/common/git-notes.html">git notes</a> <a href="#git-notes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add or inspect object notes.
> More information: <https://git-scm.com/docs/git-notes>.

#### List all notes and the objects they are attached to:
```shell
git notes list
```
#### List all notes attached to a given object (defaults to HEAD):
```shell
git notes list [{{object}}]
```
#### Show the notes attached to a given object (defaults to HEAD):
```shell
git notes show [{{object}}]
```
#### Append a note to a specified object (opens the default text editor):
```shell
git notes append {{object}}
```
#### Append a note to a specified object, specifying the message:
```shell
git notes append --message="{{message_text}}"
```
#### Edit an existing note (defaults to HEAD):
```shell
git notes edit [{{object}}]
```
#### Copy a note from one object to another:
```shell
git notes copy {{source_object}} {{target_object}}
```
#### Remove all the notes added to a specified object:
```shell
git notes remove {{object}}
```
{% endraw %}