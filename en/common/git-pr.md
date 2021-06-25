---
layout: default
title: "git pr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-pr">
  <a href="/en/common/git-pr.html">git pr</a> <a href="#git-pr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check out GitHub pull requests locally.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-pr>.

#### Check out a specific pull request:
```shell
git pr {{pr_number}}
```
#### Check out a pull request for a specific remote:
```shell
git pr {{pr_number}} {{remote}}
```
#### Check out a pull request from its URL:
```shell
git pr {{url}}
```
#### Clean up old pull request branches:
```shell
git pr clean
```
{% endraw %}