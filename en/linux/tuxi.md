---
layout: default
title: "tuxi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tuxi">
  <a href="/en/linux/tuxi.html">tuxi</a> <a href="#tuxi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI tool that scrapes Google search results and SERPs that provides instant and concise answers.
> More information: <https://github.com/Bugswriter/tuxi>.

#### Make a search using Google:
```shell
tuxi {{search_terms}}
```
#### Display the search results in [r]aw format (no pretty output, no colors):
```shell
tuxi -r {{search_terms}}
```
#### Display only search results (silences "Did you mean?", greetings and usage):
```shell
tuxi -q {{search_terms}}
```
#### Display help:
```shell
tuxi -h
```
{% endraw %}