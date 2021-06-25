---
layout: default
title: "googler"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="googler">
  <a href="/en/common/googler.html">googler</a> <a href="#googler"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search Google from command-line.
> More information: <https://github.com/jarun/googler>.

#### Search Google for a keyword:
```shell
googler {{keyword}}
```
#### Search Google and open the first result in web browser:
```shell
googler -j {{keyword}}
```
#### Show N search results (default 10):
```shell
googler -n {{N}} {{keyword}}
```
#### Disable automatic spelling correction:
```shell
googler -x {{keyword}}
```
#### Search one site for a keyword:
```shell
googler -w {{site}} {{keyword}}
```
#### Show Google search result in JSON format:
```shell
googler --json {{keyword}}
```
#### Perform in-place self-upgrade:
```shell
googler -u
```
#### For more help in interactive mode:
```shell
?
```
{% endraw %}