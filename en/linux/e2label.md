---
layout: default
title: "e2label"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="e2label">
  <a href="/en/linux/e2label.html">e2label</a> <a href="#e2label"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change the label on an ext2/ext3/ext4 filesystem.

#### Change the volume label on a specific ext partition:
```shell
e2label {{/dev/sda1}} "{{label_name}}"
```
{% endraw %}