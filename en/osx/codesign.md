---
layout: default
title: "codesign"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="codesign">
  <a href="/en/osx/codesign.html">codesign</a> <a href="#codesign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manipulate code signatures for macOS.

#### Sign an application with a certificate:
```shell
codesign -s "{{My Company Name}}" {{path/to/App.app}}
```
#### Verify the certificate of an application:
```shell
codesign -v {{path/to/App.app}}
```
{% endraw %}