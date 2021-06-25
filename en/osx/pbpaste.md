---
layout: default
title: "pbpaste"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pbpaste">
  <a href="/en/osx/pbpaste.html">pbpaste</a> <a href="#pbpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send the contents of the clipboard to standard output.

#### Write the contents of the clipboard to a file:
```shell
pbpaste > {{file}}
```
#### Use the contents of the clipboard as input to a command:
```shell
pbpaste | grep foo
```
{% endraw %}