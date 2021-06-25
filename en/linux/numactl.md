---
layout: default
title: "numactl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="numactl">
  <a href="/en/linux/numactl.html">numactl</a> <a href="#numactl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control NUMA policy for processes or shared memory.
> More information: <https://man7.org/linux/man-pages/man8/numactl.8.html>.

#### Run a command on node 0 with memory allocated on node 0 and 1:
```shell
numactl --cpunodebind={{0}} --membind={{0,1}} -- {{command}} {{command_arguments}}
```
#### Run a command on CPUs (cores) 0-4 and 8-12 of the current cpuset:
```shell
numactl --physcpubind={{+0-4,8-12}} -- {{command}} {{command_arguments}}
```
#### Run a command with its memory interleaved on all CPUs:
```shell
numactl --interleave={{all}} -- {{command}} {{command_arguments}}
```
{% endraw %}