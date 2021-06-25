---
layout: default
title: "git config"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-config">
  <a href="/en/common/git-config.html">git config</a> <a href="#git-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage custom configuration options for Git repositories.
> These configurations can be local (for the current repository) or global (for the current user).
> More information: <https://git-scm.com/docs/git-config>.

#### List only local configuration entries (stored in `.git/config` in the current repository):
```shell
git config --list --local
```
#### List only global configuration entries (stored in `~/.gitconfig`):
```shell
git config --list --global
```
#### List all configuration entries that have been defined either locally or globally:
```shell
git config --list
```
#### Get the value of a given configuration entry:
```shell
git config alias.unstage
```
#### Set the global value of a given configuration entry:
```shell
git config --global alias.unstage "reset HEAD --"
```
#### Revert a global configuration entry to its default value:
```shell
git config --global --unset alias.unstage
```
#### Edit the Git configuration for the current repository in the default editor:
```shell
git config --edit
```
#### Edit the global Git configuration in the default editor:
```shell
git config --global --edit
```
{% endraw %}