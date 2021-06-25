---
layout: default
title: "git fork"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fork">
  <a href="/en/common/git-fork.html">git fork</a> <a href="#git-fork"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fork the given GitHub repo. Like `git clone` but forks first.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-fork>.

#### Fork and clone a GitHub repository by its URL:
```shell
git fork {{https://github.com/tldr-pages/tldr}}
```
#### Fork and clone a GitHub repository by its slug:
```shell
git fork {{tldr-pages/tldr}}
```
{% endraw %}