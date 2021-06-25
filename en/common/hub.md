---
layout: default
title: "hub"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hub">
  <a href="/en/common/hub.html">hub</a> <a href="#hub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A wrapper for Git that adds commands for working with GitHub-based projects.
> If set up as instructed by `hub alias`, one can use `git` to run `hub` commands.
> More information: <https://hub.github.com>.

#### Clone a repository using its slug (owners can omit the username):
```shell
hub clone {{username}}/{{repo_name}}
```
#### Create a fork of the current repository (cloned from another user) under your GitHub profile:
```shell
hub fork
```
#### Push the current local branch to GitHub and create a PR for it in the original repository:
```shell
hub push {{remote_name}} && hub pull-request
```
#### Create a PR of the current (already pushed) branch, reusing the message from the first commit:
```shell
hub pull-request --no-edit
```
#### Create a new branch with the contents of a pull request and switch to it:
```shell
hub pr checkout {{pr_number}}
```
#### Upload the current (local-only) repository to your GitHub account:
```shell
hub create
```
#### Fetch Git objects from upstream and update local branches:
```shell
hub sync
```
{% endraw %}