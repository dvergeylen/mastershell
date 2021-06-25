---
layout: default
title: "mdutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mdutil">
  <a href="/en/osx/mdutil.html">mdutil</a> <a href="#mdutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the metadata stores used by Spotlight for indexing.

#### Show the indexing status of the startup volume:
```shell
mdutil -s {{/}}
```
#### Turn on/off the Spotlight indexing for a given volume:
```shell
mdutil -i {{on|off}} {{path/to/volume}}
```
#### Turn on/off indexing for all volumes:
```shell
mdutil -a -i {{on|off}}
```
#### Erase the metadata stores and restart the indexing process:
```shell
mdutil -E {{path/to/volume}}
```
{% endraw %}