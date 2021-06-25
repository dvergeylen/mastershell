---
layout: default
title: "dvc freeze"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-freeze">
  <a href="/en/common/dvc-freeze.html">dvc freeze</a> <a href="#dvc-freeze"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Freeze stages in the DVC pipeline.
> This prevents DVC from tracking changes in stage dependencies and re-execution until unfreeze.
> See also `dvs unfreeze`.
> More information: <https://dvc.org/doc/command-reference/freeze>.

#### Freeze 1 or more specified stages:
```shell
dvc freeze {{stage_name_a}} [{{stage_name_b}} ...]
```
{% endraw %}