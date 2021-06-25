---
layout: default
title: "git ls-remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ls-remote">
  <a href="/en/common/git-ls-remote.html">git ls-remote</a> <a href="#git-ls-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Git command for listing references in a remote repository based on name or URL.
> If no name or URL are given, then the configured upstream branch will be used, or remote origin if the former is not configured.
> More information: <https://git-scm.com/docs/git-ls-remote>.

#### Show all references in the default remote repository:
```shell
git ls-remote
```
#### Show only heads references in the default remote repository:
```shell
git ls-remote --heads
```
#### Show only tags references in the default remote repository:
```shell
git ls-remote --tags
```
#### Show all references from a remote repository based on name or URL:
```shell
git ls-remote {{repository_url}}
```
#### Show references from a remote repository filtered by a pattern:
```shell
git ls-remote {{repository_name}} "{{pattern}}"
```
{% endraw %}