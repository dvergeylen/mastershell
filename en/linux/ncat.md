---
layout: default
title: "ncat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ncat">
  <a href="/en/linux/ncat.html">ncat</a> <a href="#ncat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Use the normal `cat` functionality over networks.

#### Listen for input on the specified port and write it to the specified file:
```shell
ncat -l {{port}} > {{path/to/file}}
```
#### Accept multiple connections and keep ncat open after they have been closed:
```shell
ncat -lk {{port}}
```
#### Write output of specified file to the specified host on the specified port:
```shell
ncat {{address}} {{port}} < {{path/to/file}}
```
{% endraw %}