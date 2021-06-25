---
layout: default
title: "git for-each-repo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-for-each-repo">
  <a href="/en/common/git-for-each-repo.html">git for-each-repo</a> <a href="#git-for-each-repo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a Git command on a list of repositories.
> Note: this command is experimental and may change.
> More information: <https://git-scm.com/docs/git-for-each-repo>.

#### Run maintenance on each of a list of repositories stored in the `maintenance.repo` user configuration variable:
```shell
git for-each-repo --config={{maintenance.repo}} {{maintenance run}}
```
#### Run `git pull` on each repository listed in a global configuration variable:
```shell
git for-each-repo --config={{global_configuration_variable}} {{pull}}
```
{% endraw %}