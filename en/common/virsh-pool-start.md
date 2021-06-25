---
layout: default
title: "virsh pool-start"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-start">
  <a href="/en/common/virsh-pool-start.html">virsh pool-start</a> <a href="#virsh-pool-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Start a previously configured but inactive virtual machine storage pool.
> See also: `virsh`, `virsh-pool-define-as`, `virsh-pool-destroy`.
> More information: <https://manned.org/virsh>.

#### Start the storage pool specified by name or UUID (determine using `virsh pool-list`) and create the underlying storage system if it doesn't exist:
```shell
virsh pool-start --pool {{name|uuid}} --build
```
{% endraw %}