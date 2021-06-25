---
layout: default
title: "ncmpcpp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ncmpcpp">
  <a href="/en/common/ncmpcpp.html">ncmpcpp</a> <a href="#ncmpcpp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line music player client for the Music Player Daemon.
> More information: <https://rybczak.net/ncmpcpp>.

#### Connect to a music player daemon on a given host and port:
```shell
ncmpcpp --host {{ip}} --port {{port}}
```
#### Display metadata of the current song to console:
```shell
ncmpcpp --current-song
```
#### Use a specified configuration file:
```shell
ncmpcpp --config {{file}}
```
#### Use a different set of key bindings from a file:
```shell
ncmpcpp --bindings {{file}}
```
{% endraw %}