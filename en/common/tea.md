---
layout: default
title: "tea"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tea">
  <a href="/en/common/tea.html">tea</a> <a href="#tea"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool to interact with Gitea servers.
> More information: <https://gitea.com/gitea/tea>.

#### Log into a Gitea server:
```shell
tea login add --name "{{name}}" --url "{{url}}" --token "{{token}}"
```
#### Display all repositories:
```shell
tea repos ls
```
#### Display a list of issues:
```shell
tea issues ls
```
#### Display a list of issues for a specific repository:
```shell
tea issues ls --repo "{{repository}}"
```
#### Create a new issue:
```shell
tea issues create --title "{{title}}" --body "{{body}}"
```
#### Display a list of open pull requests:
```shell
tea pulls ls
```
#### Open the current repository in a browser:
```shell
tea open
```
{% endraw %}