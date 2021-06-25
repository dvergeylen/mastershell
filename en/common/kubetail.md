---
layout: default
title: "kubetail"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kubetail">
  <a href="/en/common/kubetail.html">kubetail</a> <a href="#kubetail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to tail multiple Kubernetes pod logs at the same time.
> More information: <https://github.com/johanhaleby/kubetail>.

#### Tail the logs of multiple pods (whose name starts with "my_app") in one go:
```shell
kubetail {{my_app}}
```
#### Tail only a specific container from multiple pods:
```shell
kubetail {{my_app}} -c {{my_container}}
```
#### To tail multiple containers from multiple pods:
```shell
kubetail {{my_app}} -c {{my_container_1}} -c {{my_container_2}}
```
#### To tail multiple applications at the same time separate them by comma:
```shell
kubetail {{my_app_1}},{{my_app_2}}
```
{% endraw %}