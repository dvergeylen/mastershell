---
layout: default
title: "sd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sd">
  <a href="/en/common/sd.html">sd</a> <a href="#sd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Intuitive find & replace CLI.

#### Trim some whitespace using a regular expression:
```shell
{{echo 'lorem ipsum 23   '}} | sd '\s+$' ''
```
#### Replace words using capture groups:
```shell
{{echo 'cargo +nightly watch'}} | sd '(\w+)\s+\+(\w+)\s+(\w+)' 'cmd: $1, channel: $2, subcmd: $3'
```
#### Find and replace in a file printing the result to stdout:
```shell
sd -p {{'window.fetch'}} {{'fetch'}} {{http.js}}
```
#### Find and replace across a project changing each file in place:
```shell
sd {{'from "react"'}} {{'from "preact"'}} $(find . -type f)
```
{% endraw %}