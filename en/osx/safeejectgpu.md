---
layout: default
title: "SafeEjectGPU"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="safeejectgpu">
  <a href="/en/osx/safeejectgpu.html">SafeEjectGPU</a> <a href="#safeejectgpu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Eject a GPU safely.
> Visit the man page for more info.

#### Eject all GPUs:
```shell
SafeEjectGPU Eject
```
#### List all GPUs attached:
```shell
SafeEjectGPU gpus
```
#### List apps using a GPU:
```shell
SafeEjectGPU gpuid {{GPU_ID}} apps
```
#### Get the status of a GPU:
```shell
SafeEjectGPU gpuid {{GPU_ID}} status
```
#### Eject a GPU:
```shell
SafeEjectGPU gpuid {{GPU_ID}} Eject
```
#### Launch an app on a GPU:
```shell
SafeEjectGPU gpuid {{GPU_ID}} LaunchOnGPU {{path/to/App.app}}
```
{% endraw %}