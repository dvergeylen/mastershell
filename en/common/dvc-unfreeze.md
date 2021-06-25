---
layout: default
title: "dvc unfreeze"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-unfreeze">
  <a href="/en/common/dvc-unfreeze.html">dvc unfreeze</a> <a href="#dvc-unfreeze"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Unfreeze stages in the DVC pipeline.
> This allows DVC to start tracking changes in stage dependencies again after they were frozen.
> See also `dvc freeze`.
> More information: <https://dvc.org/doc/command-reference/unfreeze>.

#### Unfreeze 1 or more specified stages:
```shell
dvc unfreeze {{stage_name_a}} [{{stage_name_b}} ...]
```
{% endraw %}