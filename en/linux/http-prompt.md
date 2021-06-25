---
layout: default
title: "http-prompt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="http-prompt">
  <a href="/en/linux/http-prompt.html">http-prompt</a> <a href="#http-prompt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An interactive command-line HTTP client featuring autocomplete and syntax highlighting.

#### Launch a session targeting the default URL of http://localhost:8000 or the previous session:
```shell
http-prompt
```
#### Launch a session with a given URL:
```shell
http-prompt {{http://example.com}}
```
#### Launch a session with some initial options:
```shell
http-prompt {{localhost:8000/api}} --auth {{username:password}}
```
{% endraw %}