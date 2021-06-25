---
layout: default
title: "gh repo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-repo">
  <a href="/en/common/gh-repo.html">gh repo</a> <a href="#gh-repo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Work with GitHub repositories on the command-line.
> More information: <https://cli.github.com/manual/gh_repo>.

#### Create a new repository (if the repository name is not set, the default name will be the name of the current directory):
```shell
gh repo create {{name}}
```
#### Clone a repository:
```shell
gh repo clone {{owner}}/{{repository}}
```
#### Fork and clone a repository:
```shell
gh repo fork {{owner}}/{{repository}} --clone
```
#### View a repository in the web browser:
```shell
gh repo view {{repository}} --web
```
#### List repositories owned by a specific user or organization (if the owner is not set, the default owner will be the currently logged in user):
```shell
gh repo list {{owner}}
```
#### List only non-forks repositories:
```shell
gh repo list {{owner}} --non-forks
```
#### List repositories with a specific primary coding language:
```shell
gh repo list {{owner}} --language {{language_name}}
```
{% endraw %}