---
layout: default
title: "git remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-remote">
  <a href="/en/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage set of tracked repositories ("remotes").
> More information: <https://git-scm.com/docs/git-remote>.

#### Show a list of existing remotes, their names and URL:
```shell
git remote -v
```
#### Show information about a remote:
```shell
git remote show {{remote_name}}
```
#### Add a remote:
```shell
git remote add {{remote_name}} {{remote_url}}
```
#### Change the URL of a remote (use `--add` to keep the existing URL):
```shell
git remote set-url {{remote_name}} {{new_url}}
```
#### Remove a remote:
```shell
git remote remove {{remote_name}}
```
#### Rename a remote:
```shell
git remote rename {{old_name}} {{new_name}}
```
{% endraw %}