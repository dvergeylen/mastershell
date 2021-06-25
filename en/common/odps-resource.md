---
layout: default
title: "odps resource"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="odps-resource">
  <a href="/en/common/odps-resource.html">odps resource</a> <a href="#odps-resource"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage resources in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

#### Show resources in the current project:
```shell
list resources;
```
#### Add file resource:
```shell
add file {{filename}} as {{alias}};
```
#### Add archive resource:
```shell
add archive {{archive.tar.gz}} as {{alias}};
```
#### Add .jar resource:
```shell
add jar {{package.jar}};
```
#### Add .py resource:
```shell
add py {{script.py}};
```
#### Delete resource:
```shell
drop resource {{resource_name}};
```
{% endraw %}