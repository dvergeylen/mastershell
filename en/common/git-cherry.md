---
layout: default
title: "git cherry"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cherry">
  <a href="/en/common/git-cherry.html">git cherry</a> <a href="#git-cherry"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find commits that have yet to be applied upstream.
> More information: <https://git-scm.com/docs/git-cherry>.

#### Show commits (and their messages) with equivalent commits upstream:
```shell
git cherry -v
```
#### Specify a different upstream and topic branch:
```shell
git cherry {{origin}} {{topic}}
```
#### Limit commits to those within a given limit:
```shell
git cherry {{origin}} {{topic}} {{base}}
```
{% endraw %}