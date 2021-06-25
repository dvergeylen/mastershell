---
layout: default
title: "gh completion"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-completion">
  <a href="/en/common/gh-completion.html">gh completion</a> <a href="#gh-completion"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate shell completion scripts for GitHub CLI commands.
> More information: <https://cli.github.com/manual/gh_completion>.

#### Display the subcommand help:
```shell
gh completion
```
#### Print a completion script:
```shell
gh completion --shell {{bash|zsh|fish|powershell}}
```
#### Append the `gh` completion script to `~/.bashrc`:
```shell
gh completion --shell {{bash}} >> {{~/.bashrc}}
```
#### Append the `gh` completion script to `~/.zshrc`:
```shell
gh completion --shell {{zsh}} >> {{~/.zshrc}}
```
{% endraw %}