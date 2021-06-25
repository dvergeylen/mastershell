---
layout: default
title: "nf-core"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nf-core">
  <a href="/en/common/nf-core.html">nf-core</a> <a href="#nf-core"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The nf-core framework tools, to create, check and develop best-practice guidelines for Nextflow.
> More information: <https://nf-co.re/tools>.

#### List existing pipelines on nf-core:
```shell
nf-core list
```
#### Create a new pipeline skeleton:
```shell
nf-core create
```
#### Lint the pipeline code:
```shell
nf-core lint {{path/to/directory}}
```
#### Bump software versions in pipeline recipe:
```shell
nf-core bump-version {{path/to/directory}} {{new_version}}
```
#### Launch an nf-core pipeline:
```shell
nf-core launch {{pipeline_name}}
```
#### Download an nf-core pipeline for offline use:
```shell
nf-core download {{pipeline_name}}
```
{% endraw %}