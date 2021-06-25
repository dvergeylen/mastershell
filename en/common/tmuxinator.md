---
layout: default
title: "tmuxinator"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tmuxinator">
  <a href="/en/common/tmuxinator.html">tmuxinator</a> <a href="#tmuxinator"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manage tmux sessions easily.
> More information: <https://github.com/tmuxinator/tmuxinator>.

#### Create a new project:
```shell
tmuxinator new {{project}}
```
#### Edit a project:
```shell
tmuxinator edit {{project}}
```
#### List projects:
```shell
tmuxinator list
```
#### Start a tmux session based on project:
```shell
tmuxinator start {{project}}
```
#### Stop a project's tmux session:
```shell
tmuxinator stop {{project}}
```
{% endraw %}