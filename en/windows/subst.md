---
layout: default
title: "subst"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="subst">
  <a href="/en/windows/subst.html">subst</a> <a href="#subst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Associates a path with a virtual drive letter.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/subst>.

#### List active associations:
```shell
subst
```
#### Add an association:
```shell
subst {{Z:}} {{C:\Python2.7}}
```
#### Remove an association:
```shell
subst {{Z:}} /d
```
{% endraw %}