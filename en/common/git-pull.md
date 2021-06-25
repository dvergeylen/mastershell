---
layout: default
title: "git pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-pull">
  <a href="/en/common/git-pull.html">git pull</a> <a href="#git-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fetch branch from a remote repository and merge it to local repository.
> More information: <https://git-scm.com/docs/git-pull>.

#### Download changes from default remote repository and merge it:
```shell
git pull
```
#### Download changes from default remote repository and use fast forward:
```shell
git pull --rebase
```
#### Download changes from given remote repository and branch, then merge them into HEAD:
```shell
git pull {{remote_name}} {{branch}}
```
{% endraw %}