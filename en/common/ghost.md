---
layout: default
title: "ghost"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ghost">
  <a href="/en/common/ghost.html">ghost</a> <a href="#ghost"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A blogging platform and headless CMS.
> More information: <https://ghost.org>.

#### Install Ghost in the current directory:
```shell
ghost install
```
#### Start an instance of Ghost:
```shell
ghost start
```
#### Restart the Ghost instance:
```shell
ghost restart
```
#### Check the system for any potential hiccups while installing or updating Ghost:
```shell
ghost doctor
```
#### View the logs of a Ghost instance:
```shell
ghost log {{name}}
```
#### Run a Ghost instance directly (used by process managers and for debugging):
```shell
ghost run
```
#### View running Ghost processes:
```shell
ghost ls
```
#### View or edit Ghost configuration:
```shell
ghost config {{key}} {{value}}
```
{% endraw %}