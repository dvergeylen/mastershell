---
layout: default
title: "git mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-mv">
  <a href="/en/common/git-mv.html">git mv</a> <a href="#git-mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Move or rename files and update the Git index.
> More information: <https://git-scm.com/docs/git-mv>.

#### Move file inside the repo and add the movement to the next commit:
```shell
git mv {{path/to/file}} {{new/path/to/file}}
```
#### Rename file and add renaming to the next commit:
```shell
git mv {{filename}} {{new_filename}}
```
#### Overwrite the file in the target path if it exists:
```shell
git mv --force {{file}} {{target}}
```
{% endraw %}