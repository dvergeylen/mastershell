---
layout: default
title: "while"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="while">
  <a href="/en/common/while.html">while</a> <a href="#while"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple shell loop.

#### Read stdin and perform an action on every line:
```shell
while read line; do echo "$line"; done
```
#### Execute a command forever once every second:
```shell
while :; do {{command}}; sleep 1; done
```
{% endraw %}