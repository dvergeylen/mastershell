---
layout: default
title: "odps inst"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="odps-inst">
  <a href="/en/common/odps-inst.html">odps inst</a> <a href="#odps-inst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage instances in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

#### Show instances created by current user:
```shell
show instances;
```
#### Describe the details of an instance:
```shell
desc instance {{instance_id}};
```
#### Check the status of an instance:
```shell
status {{instance_id}};
```
#### Wait on the termination of an instance, printing log and progress information until then:
```shell
wait {{instance_id}};
```
#### Kill an instance:
```shell
kill {{instance_id}};
```
{% endraw %}