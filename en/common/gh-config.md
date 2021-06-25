---
layout: default
title: "gh config"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-config">
  <a href="/en/common/gh-config.html">gh config</a> <a href="#gh-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change configuration for GitHub cli.
> More information: <https://cli.github.com/manual/gh_config>.

#### Display what Git protocol is being used:
```shell
gh config get git_protocol
```
#### Set protocol to SSH:
```shell
gh config set git_protocol {{ssh}}
```
#### Use `delta` in side-by-side mode as the default pager for all `gh` commands:
```shell
gh config set pager '{{delta --side-by-side}}'
```
#### Set text editor to Vim:
```shell
gh config set editor {{vim}}
```
#### Reset to default text editor:
```shell
gh config set editor {{""}}
```
#### Disable interactive prompts:
```shell
gh config set prompt {{disabled}}
```
#### Set a specific configuration value:
```shell
gh config set {{key}} {{value}}
```
{% endraw %}