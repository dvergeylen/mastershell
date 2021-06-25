---
layout: default
title: "tuir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tuir">
  <a href="/en/common/tuir.html">tuir</a> <a href="#tuir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text user-interface (TUI) to view and interact with Reddit from your terminal.
> Navigate with the Vim keys.
> More information: <https://gitlab.com/ajak/tuir>.

#### Launch tuir:
```shell
tuir
```
#### Open a subreddit:
```shell
/{{subreddit_name}}
```
#### Open a link:
```shell
o
```
#### Open a specific subreddit on launch:
```shell
tuir -s {{subreddit_name}}
```
#### Open external links using programs defined in the mailcap config:
```shell
tuir --enable-media
```
{% endraw %}