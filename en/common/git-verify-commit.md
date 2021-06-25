---
layout: default
title: "git verify-commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-verify-commit">
  <a href="/en/common/git-verify-commit.html">git verify-commit</a> <a href="#git-verify-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check for GPG verification of commits.
> If no commits are verified, nothing will be printed, regardless of options specified.
> More information: <https://git-scm.com/docs/git-verify-commit>.

#### Check commits for a GPG signature:
```shell
git verify-commit {{commit_hash1 optional_commit_hash2 ...}}
```
#### Check commits for a GPG signature and show details of each commit:
```shell
git verify-commit {{commit_hash1 optional_commit_hash2 ...}} --verbose
```
#### Check commits for a GPG signature and print the raw details:
```shell
git verify-commit {{commit_hash1 optional_commit_hash2 ...}} --raw
```
{% endraw %}