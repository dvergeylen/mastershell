---
layout: default
title: "which"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="which">
  <a href="/en/common/which.html">which</a> <a href="#which"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Locate a program in the user's path.

#### Search the PATH environment variable and display the location of any matching executables:
```shell
which {{executable}}
```
#### If there are multiple executables which match, display all:
```shell
which -a {{executable}}
```
{% endraw %}