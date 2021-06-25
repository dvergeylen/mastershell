---
layout: default
title: "gh pr merge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-pr-merge">
  <a href="/en/common/gh-pr-merge.html">gh pr merge</a> <a href="#gh-pr-merge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Merge GitHub pull requests.
> More information: <https://cli.github.com/manual/gh_pr_merge>.

#### Merge the pull request associated with the current branch interactively:
```shell
gh pr merge
```
#### Merge the specified pull request, interactively:
```shell
gh pr merge {{pr_number}}
```
#### Merge the pull request, removing the branch on both the local and the remote:
```shell
gh pr merge --delete-branch
```
#### Merge the current pull request with the specified merge strategy:
```shell
gh pr merge --{{merge|squash|rebase}}
```
#### Squash the current pull request into one commit with the message body and merge:
```shell
gh pr merge --squash --body="{{commit_message_body}}"
```
#### Display help:
```shell
gh pr merge --help
```
{% endraw %}