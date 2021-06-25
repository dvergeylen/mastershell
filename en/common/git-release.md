---
layout: default
title: "git release"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-release">
  <a href="/en/common/git-release.html">git release</a> <a href="#git-release"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a Git tag for a release.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-release>.

#### Create and push a release:
```shell
git release {{tag_name}}
```
#### Create and push a signed release:
```shell
git release {{tag_name}} -s
```
#### Create and push a release with a message:
```shell
git release {{{tag_name}}} -m "{{message}}"
```
{% endraw %}