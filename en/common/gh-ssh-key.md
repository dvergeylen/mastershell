---
layout: default
title: "gh ssh-key"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-ssh-key">
  <a href="/en/common/gh-ssh-key.html">gh ssh-key</a> <a href="#gh-ssh-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage GitHub SSH keys from the command-line.
> More information: <https://cli.github.com/manual/gh_ssh-key>.

#### Display help:
```shell
gh ssh-key
```
#### List SSH keys for the currently authenticated user:
```shell
gh ssh-key list
```
#### Add an SSH key to the currently authenticated user's account:
```shell
gh ssh-key add {{path/to/key.pub}}
```
#### Add an SSH key to the currently authenticated user's account with a specific title:
```shell
gh ssh-key add --title {{title}} {{path/to/key.pub}}
```
{% endraw %}