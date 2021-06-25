---
layout: default
title: "git update-ref"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-update-ref">
  <a href="/en/common/git-update-ref.html">git update-ref</a> <a href="#git-update-ref"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Git command for creating, updating, and deleting Git refs.
> More information: <https://git-scm.com/docs/git-update-ref>.

#### Delete a ref, useful for soft resetting the first commit:
```shell
git update-ref -d {{HEAD}}
```
#### Update ref with a message:
```shell
git update-ref -m {{message}} {{HEAD}} {{4e95e05}}
```
{% endraw %}