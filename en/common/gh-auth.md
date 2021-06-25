---
layout: default
title: "gh auth"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-auth">
  <a href="/en/common/gh-auth.html">gh auth</a> <a href="#gh-auth"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Authenticate with a GitHub host from the command-line.
> More information: <https://cli.github.com/manual/gh_auth>.

#### Log in with interactive prompt:
```shell
gh auth login
```
#### Log in with a token from standard input (created in https://github.com/settings/tokens):
```shell
echo {{your_token}} | gh auth login --with-token
```
#### Check if you are logged in:
```shell
gh auth status
```
#### Log out:
```shell
gh auth logout
```
#### Log in with a specific GitHub Enterprise Server:
```shell
gh auth login --hostname {{github.example.com}}
```
#### Refresh the session to ensure authentication credentials have the correct minimum scopes (removes additional scopes requested previously):
```shell
gh auth refresh
```
#### Expand the permission scopes:
```shell
gh auth refresh --scopes {{write:org,read:public_key}}
```
{% endraw %}