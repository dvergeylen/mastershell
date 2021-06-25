---
layout: default
title: "tig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tig">
  <a href="/en/common/tig.html">tig</a> <a href="#tig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text-mode interface for Git.
> More information: <https://github.com/jonas/tig>.

#### Show the sequence of commits starting from the current one in reverse chronological order:
```shell
tig
```
#### Show the history of a specific branch:
```shell
tig {{branch}}
```
#### Show the history of specific files or directories:
```shell
tig {{path1 path2 …}}
```
#### Show the difference between two references (such as branches or tags):
```shell
tig {{base_ref}}..{{compared_ref}}
```
#### Display commits from all branches and stashes:
```shell
tig --all
```
#### Start in stash view, displaying all saved stashes:
```shell
tig stash
```
{% endraw %}