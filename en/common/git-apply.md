---
layout: default
title: "git apply"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-apply">
  <a href="/en/common/git-apply.html">git apply</a> <a href="#git-apply"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apply a patch to files and/or to the index.
> More information: <https://git-scm.com/docs/git-apply>.

#### Print messages about the patched files:
```shell
git apply --verbose {{path/to/file}}
```
#### Apply and add the patched files to the index:
```shell
git apply --index {{path/to/file}}
```
#### Apply a remote patch file:
```shell
curl {{https://example.com/file.patch}} | git apply
```
#### Output diffstat for the input and apply the patch:
```shell
git apply --stat --apply {{path/to/file}}
```
#### Apply the patch in reverse:
```shell
git apply --reverse {{path/to/file}}
```
#### Store the patch result in the index without modifying the working tree:
```shell
git apply --cache {{path/to/file}}
```
{% endraw %}