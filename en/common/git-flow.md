---
layout: default
title: "git flow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-flow">
  <a href="/en/common/git-flow.html">git flow</a> <a href="#git-flow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A collection of Git extensions to provide high-level repository operations.
> More information: <https://github.com/nvie/gitflow>.

#### Initialize it inside an existing Git repository:
```shell
git flow init
```
#### Start developing on a feature branch based on `develop`:
```shell
git flow feature start {{feature}}
```
#### Finish development on a feature branch, merging it into the `develop` branch and deleting it:
```shell
git flow feature finish {{feature}}
```
#### Publish a feature to the remote server:
```shell
git flow feature publish {{feature}}
```
#### Get a feature published by another user:
```shell
git flow feature pull origin {{feature}}
```
{% endraw %}