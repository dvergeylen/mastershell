---
layout: default
title: "git show-ref"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show-ref">
  <a href="/en/common/git-show-ref.html">git show-ref</a> <a href="#git-show-ref"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Git command for listing references.
> More information: <https://git-scm.com/docs/git-show-ref>.

#### Show all refs in the repository:
```shell
git show-ref
```
#### Show only heads references:
```shell
git show-ref --heads
```
#### Show only tags references:
```shell
git show-ref --tags
```
#### Verify that a given reference exists:
```shell
git show-ref --verify {{path/to/ref}}
```
{% endraw %}