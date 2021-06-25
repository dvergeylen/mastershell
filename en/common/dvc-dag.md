---
layout: default
title: "dvc dag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dvc-dag">
  <a href="/en/common/dvc-dag.html">dvc dag</a> <a href="#dvc-dag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visualize the pipeline(s) defined in `dvc.yaml`.
> More information: <https://dvc.org/doc/command-reference/dag>.

#### Visualize the entire pipeline:
```shell
dvc dag
```
#### Visualize the pipeline stages up to a specified target stage:
```shell
dvc dag {{target}}
```
#### Export the pipeline in the dot format:
```shell
dvc dag --dot > {{path/to/pipeline.dot}}
```
{% endraw %}