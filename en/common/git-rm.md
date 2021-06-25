---
layout: default
title: "git rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rm">
  <a href="/en/common/git-rm.html">git rm</a> <a href="#git-rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove files from repository index and local filesystem.
> More information: <https://git-scm.com/docs/git-rm>.

#### Remove file from repository index and filesystem:
```shell
git rm {{file}}
```
#### Remove directory:
```shell
git rm -r {{directory}}
```
#### Remove file from repository index but keep it untouched locally:
```shell
git rm --cached {{file}}
```
{% endraw %}