---
layout: default
title: "link"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="link">
  <a href="/en/common/link.html">link</a> <a href="#link"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a hard link to an existing file.
> For more options, see the `ln` command.
> More information: <https://www.gnu.org/software/coreutils/link>.

#### Create a hard link from a new file to an existing file:
```shell
link {{path/to/existing_file}} {{path/to/new_file}}
```
{% endraw %}