---
layout: default
title: "git column"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-column">
  <a href="/en/common/git-column.html">git column</a> <a href="#git-column"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display data in columns.
> More information: <https://git-scm.com/docs/git-column>.

#### Format the standard input as multiple columns:
```shell
ls | git column --mode={{column}}
```
#### Format the standard input as multiple columns with a maximum width of `100`:
```shell
ls | git column --mode=column --width={{100}}
```
#### Format the standard input as multiple columns with a maximum padding of `30`:
```shell
ls | git column --mode=column --padding={{30}}
```
{% endraw %}