---
layout: default
title: "git reflog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reflog">
  <a href="/en/common/git-reflog.html">git reflog</a> <a href="#git-reflog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show a log of changes to local references like HEAD, branches or tags.
> More information: <https://git-scm.com/docs/git-reflog>.

#### Show the reflog for HEAD:
```shell
git reflog
```
#### Show the reflog for a given branch:
```shell
git reflog {{branch_name}}
```
#### Show only the 5 latest entries in the reflog:
```shell
git reflog -n {{5}}
```
{% endraw %}