---
layout: default
title: "kube-fzf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kube-fzf">
  <a href="/en/common/kube-fzf.html">kube-fzf</a> <a href="#kube-fzf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shell commands for command-line fuzzy searching of Kubernetes Pods.
> See also `kubectl` for related commands.
> More information: <https://github.com/thecasualcoder/kube-fzf>.

#### Get pod details (from current namespace):
```shell
findpod
```
#### Get pod details (from all namespaces):
```shell
findpod -a
```
#### Describe a pod:
```shell
describepod
```
#### Tail pod logs:
```shell
tailpod
```
#### Exec into a pod's container:
```shell
execpod {{shell_command}}
```
#### Port-forward a pod:
```shell
pfpod {{port_number}}
```
{% endraw %}