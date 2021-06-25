---
layout: default
title: "gh pr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-pr">
  <a href="/en/common/gh-pr.html">gh pr</a> <a href="#gh-pr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage GitHub pull requests from the command-line.
> More information: <https://cli.github.com/manual/gh_pr>.

#### Create a pull request:
```shell
gh pr create
```
#### Check out a pull request locally:
```shell
gh pr checkout {{pr_number}}
```
#### View the changes made in the PR:
```shell
gh pr diff
```
#### Approve the pull request of the current branch:
```shell
gh pr review --approve
```
#### Merge the pull request associated with the current branch interactively:
```shell
gh pr merge
```
#### Edit a pull request interactively:
```shell
gh pr edit
```
#### Edit the base branch of a pull request:
```shell
gh pr edit --base {{branch_name}}
```
{% endraw %}