---
layout: default
title: "stolonctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stolonctl">
  <a href="/en/common/stolonctl.html">stolonctl</a> <a href="#stolonctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for Stolon, a cloud native PostgreSQL manager for PostgreSQL high availability.
> More information: <https://github.com/sorintlab/stolon>.

#### Get cluster status:
```shell
stolonctl --cluster-name {{cluster_name}} --store-backend {{store_backend}} --store-endpoints {{store_endpoints}} status
```
#### Get cluster data:
```shell
stolonctl --cluster-name {{cluster_name}} --store-backend {{store_backend}} --store-endpoints {{store_endpoints}} clusterdata
```
#### Get cluster specification:
```shell
stolonctl --cluster-name {{cluster_name}} --store-backend {{store_backend}} --store-endpoints {{store_endpoints}} spec
```
#### Update cluster specification with a patch in json format:
```shell
stolonctl --cluster-name {{cluster_name}} --store-backend {{store_backend}} --store-endpoints {{store_endpoints}} update --patch '{{cluster_spec}}'
```
{% endraw %}