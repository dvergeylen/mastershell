---
layout: default
title: "pushd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pushd">
  <a href="/en/windows/pushd.html">pushd</a> <a href="#pushd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Place a directory on a stack so it can be accessed later.
> See also `popd` to switch back to original directory.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/pushd>.

#### Switch to directory and push it on the stack:
```shell
pushd {{directory}}
```
{% endraw %}