---
layout: default
title: "gh issue"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-issue">
  <a href="/en/common/gh-issue.html">gh issue</a> <a href="#gh-issue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage GitHub issues from the command-line.
> More information: <https://cli.github.com/manual/gh_issue>.

#### Print out the issue:
```shell
gh issue view {{issue_number}}
```
#### Create a new issue in the web browser:
```shell
gh issue create --web
```
#### List the last 10 issues with the `bug` label:
```shell
gh issue list --limit {{10}} --label "{{bug}}"
```
#### List closed issues made by a specific user:
```shell
gh issue list --state closed --author {{username}}
```
#### Display the status of issues relevant to the user, in a specific repository:
```shell
gh issue status --repo {{owner}}/{{repository}}
```
#### Reopen an issue:
```shell
gh issue reopen {{issue_number}}
```
{% endraw %}