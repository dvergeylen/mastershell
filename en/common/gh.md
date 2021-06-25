---
layout: default
title: "gh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh">
  <a href="/en/common/gh.html">gh</a> <a href="#gh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Work seamlessly with GitHub from the command-line.
> More information: <https://cli.github.com/>.

#### Clone a GitHub repository locally:
```shell
gh repo clone {{owner}}/{{repository}}
```
#### Create a new issue:
```shell
gh issue create
```
#### View and filter the open issues of the current repository:
```shell
gh issue list
```
#### View an issue in the browser:
```shell
gh issue view --web {{issue_number}}
```
#### Create a pull request:
```shell
gh pr create
```
#### View a pull request in the browser:
```shell
gh pr view --web {{pr_number}}
```
#### Locally check out the branch of a pull request, given its number:
```shell
gh pr checkout {{pr_number}}
```
#### Check the status of a repository's pull requests:
```shell
gh pr status
```
{% endraw %}