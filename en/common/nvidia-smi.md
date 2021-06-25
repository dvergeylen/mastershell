---
layout: default
title: "nvidia-smi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nvidia-smi">
  <a href="/en/common/nvidia-smi.html">nvidia-smi</a> <a href="#nvidia-smi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aid the management and monitoring of NVIDIA GPU devices.
> More information: <https://developer.nvidia.com/nvidia-system-management-interface>.

#### Display information on all available GPUs and processes using them:
```shell
nvidia-smi
```
#### Display more detailed GPU information:
```shell
nvidia-smi --query
```
#### Monitor overall GPU usage with 1-second update interval:
```shell
nvidia-smi dmon
```
{% endraw %}