---
layout: default
title: "git authors"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-authors">
  <a href="/en/common/git-authors.html">git authors</a> <a href="#git-authors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a list of committers of a Git repository.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-authors>.

#### Print a full list of committers to stdout instead of to the `AUTHORS` file:
```shell
git authors --list
```
#### Append the list of committers to the the `AUTHORS` file and open it in the default editor:
```shell
git authors
```
#### Append the list of committers, excluding emails, to the the `AUTHORS` file and open it in the default editor:
```shell
git authors --no-email
```
{% endraw %}