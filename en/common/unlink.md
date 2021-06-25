---
layout: default
title: "unlink"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unlink">
  <a href="/en/common/unlink.html">unlink</a> <a href="#unlink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove a link to a file from the filesystem.
> The file contents is lost if the link is the last one to the file.
> More information: <https://www.gnu.org/software/coreutils/unlink>.

#### Remove the specified file if it is the last link:
```shell
unlink {{path/to/file}}
```
{% endraw %}