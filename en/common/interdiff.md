---
layout: default
title: "interdiff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="interdiff">
  <a href="/en/common/interdiff.html">interdiff</a> <a href="#interdiff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show differences between two diff files.
> More information: <http://freshmeat.sourceforge.net/projects/patchutils>.

#### Compare diff files:
```shell
interdiff {{old_file}} {{new_file}}
```
#### Compare diff files, ignoring whitespace:
```shell
interdiff -w {{old_file}} {{new_file}}
```
{% endraw %}