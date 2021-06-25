---
layout: default
title: "forever"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="forever">
  <a href="/en/common/forever.html">forever</a> <a href="#forever"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Server-side JavaScript application that makes sure Node.js applications run indefinitely (restarts after exit).
> More information: <https://github.com/foreversd/forever>.

#### Start running a file forever (as a daemon):
```shell
forever {{script}}
```
#### List running "forever" processes (along with IDs and other details of "forever" processes):
```shell
forever list
```
#### Stop a running "forever" process:
```shell
forever stop {{ID|pid|script}}
```
{% endraw %}