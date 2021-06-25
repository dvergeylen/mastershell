---
layout: default
title: "git format-patch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-format-patch">
  <a href="/en/common/git-format-patch.html">git format-patch</a> <a href="#git-format-patch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prepare .patch files. Useful when emailing commits elsewhere.
> See also `git am`, which can apply generated .patch files.
> More information: <https://git-scm.com/docs/git-format-patch>.

#### Create an auto-named `.patch` file for all the unpushed commits:
```shell
git format-patch {{origin}}
```
#### Write a `.patch` file for all the commits between 2 revisions to stdout:
```shell
git format-patch {{revision_1}}..{{revision_2}}
```
#### Write a `.patch` file for the 3 latest commits:
```shell
git format-patch -{{3}}
```
{% endraw %}