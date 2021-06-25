---
layout: default
title: "tldr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tldr">
  <a href="/en/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays simple help pages for command-line tools, from the tldr-pages project.
> More information: <https://tldr.sh>.

#### Show the tldr page for a command (hint: this is how you got here!):
```shell
tldr {{command}}
```
#### Show the tldr page for `cd`, overriding the default platform:
```shell
tldr -p {{android|linux|osx|sunos|windows}} {{cd}}
```
#### Show the tldr page for a subcommand:
```shell
tldr {{git-checkout}}
```
#### Update local pages (if the client supports caching):
```shell
tldr -u
```
{% endraw %}