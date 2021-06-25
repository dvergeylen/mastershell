---
layout: default
title: "tmux"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tmux">
  <a href="/en/common/tmux.html">tmux</a> <a href="#tmux"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminal multiplexer. It allows multiple sessions with windows, panes, and more.
> More information: <https://github.com/tmux/tmux>.

#### Start a new session:
```shell
tmux
```
#### Start a new named session:
```shell
tmux new -s {{name}}
```
#### List existing sessions:
```shell
tmux ls
```
#### Attach to the most recently used session:
```shell
tmux attach
```
#### Detach from the current session (inside a tmux session):
```shell
Ctrl-B d
```
#### Create a new window (inside a tmux session):
```shell
Ctrl-B c
```
#### Switch between sessions and windows (inside a tmux session):
```shell
Ctrl-B w
```
#### Kill a session by name:
```shell
tmux kill-session -t {{name}}
```
{% endraw %}