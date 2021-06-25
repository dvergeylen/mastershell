---
layout: default
title: "screen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="screen">
  <a href="/en/common/screen.html">screen</a> <a href="#screen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hold a session open on a remote server. Manage multiple windows with a single SSH connection.

#### Start a new screen session:
```shell
screen
```
#### Start a new named screen session:
```shell
screen -S {{session_name}}
```
#### Start a new daemon and log the output to `screenlog.x`:
```shell
screen -dmLS {{session_name}} {{command}}
```
#### Show open screen sessions:
```shell
screen -ls
```
#### Reattach to an open screen:
```shell
screen -r {{session_name}}
```
#### Detach from inside a screen:
```shell
Ctrl + A, D
```
#### Kill the current screen session:
```shell
Ctrl + A, K
```
#### Kill a detached screen:
```shell
screen -X -S {{session_name}} quit
```
{% endraw %}