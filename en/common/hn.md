---
layout: default
title: "hn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hn">
  <a href="/en/common/hn.html">hn</a> <a href="#hn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface for Hacker News.
> More information: <https://github.com/rafaelrinaldi/hn-cli>.

#### View stories on Hacker News:
```shell
hn
```
#### View _number_ of stories on Hacker News:
```shell
hn --limit {{number}}
```
#### View stories on Hacker News, and keep the list open after selecting a link:
```shell
hn --keep-open
```
#### View stories on Hacker News sorted by submission date:
```shell
hn --latest
```
{% endraw %}