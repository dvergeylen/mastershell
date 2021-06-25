---
layout: default
title: "git blame"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-blame">
  <a href="/en/common/git-blame.html">git blame</a> <a href="#git-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show commit hash and last author on each line of a file.
> More information: <https://git-scm.com/docs/git-blame>.

#### Print file with author name and commit hash on each line:
```shell
git blame {{file}}
```
#### Print file with author email and commit hash on each line:
```shell
git blame -e {{file}}
```
{% endraw %}