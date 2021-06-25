---
layout: default
title: "rsstail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rsstail">
  <a href="/en/common/rsstail.html">rsstail</a> <a href="#rsstail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `tail` for RSS feeds.
> More information: <https://github.com/gvalkov/rsstail.py>.

#### Show the feed of a given URL and wait for new entries appearing at the bottom:
```shell
rsstail -u {{url}}
```
#### Show the feed in reverse chronological order (newer at the bottom):
```shell
rsstail -r -u {{url}}
```
#### Include publication date and link:
```shell
rsstail -pl -u {{url}}
```
#### Set update interval:
```shell
rsstail -u {{url}} -i {{interval_in_seconds}}
```
#### Show feed and exit:
```shell
rsstail -1 -u {{url}}
```
{% endraw %}