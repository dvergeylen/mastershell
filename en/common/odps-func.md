---
layout: default
title: "odps func"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="odps-func">
  <a href="/en/common/odps-func.html">odps func</a> <a href="#odps-func"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage functions in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

#### Show functions in the current project:
```shell
list functions;
```
#### Create a Java function using a `.jar` resource:
```shell
create function {{func_name}} as {{path.to.package.Func}} using '{{package.jar}}';
```
#### Create a Python function using a `.py` resource:
```shell
create function {{func_name}} as {{script.Func}} using '{{script.py}}';
```
#### Delete a function:
```shell
drop function {{func_name}};
```
{% endraw %}