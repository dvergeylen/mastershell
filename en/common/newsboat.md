---
layout: default
title: "newsboat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="newsboat">
  <a href="/en/common/newsboat.html">newsboat</a> <a href="#newsboat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An RSS/Atom feed reader for text terminals.
> More information: <https://newsboat.org/>.

#### First import feed URLs from an OPML file:
```shell
newsboat -i {{my-feeds.xml}}
```
#### Alternatively, add feeds manually:
```shell
echo {{http://example.com/path/to/feed}} >> "${HOME}/.newsboat/urls"
```
#### Start newsboat and refresh all feeds on startup:
```shell
newsboat -r
```
#### See keyboard shortcuts (the most relevant are visible in the status line):
```shell
?
```
{% endraw %}