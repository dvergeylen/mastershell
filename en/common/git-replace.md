---
layout: default
title: "git replace"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-replace">
  <a href="/en/common/git-replace.html">git replace</a> <a href="#git-replace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, list, and delete refs to replace objects.
> More information: <https://git-scm.com/docs/git-replace>.

#### Replace any commit with a different one, leaving other commits unchanged:
```shell
git replace {{object}} {{replacement}}
```
#### Delete existing replace refs for the given objects:
```shell
git replace --delete {{object}}
```
#### Edit an object’s content interactively:
```shell
git replace --edit {{object}}
```
{% endraw %}