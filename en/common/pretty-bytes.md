---
layout: default
title: "pretty-bytes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pretty-bytes">
  <a href="/en/common/pretty-bytes.html">pretty-bytes</a> <a href="#pretty-bytes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert bytes to a human readable string.
> More information: <https://github.com/sindresorhus/pretty-bytes-cli>.

#### Convert numeric bytes value to a human readable string:
```shell
pretty-bytes {{1337}}
```
#### Convert numeric bytes value from stdin to a human readable string:
```shell
echo {{1337}} | pretty-bytes
```
#### Display help and usage information:
```shell
pretty-bytes --help
```
{% endraw %}