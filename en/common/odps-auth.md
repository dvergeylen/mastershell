---
layout: default
title: "odps auth"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="odps-auth">
  <a href="/en/common/odps-auth.html">odps auth</a> <a href="#odps-auth"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> User authorities in ODPS (Open Data Processing Service).
> See also `odps`.
> More information: <https://www.alibabacloud.com/help/doc-detail/27971.htm>.

#### Add a user to the current project:
```shell
add user {{username}};
```
#### Grant a set of authorities to a user:
```shell
grant {{action_list}} on {{object_type}} {{object_name}} to user {{username}};
```
#### Show authorities of a user:
```shell
show grants for {{username}};
```
#### Create a user role:
```shell
create role {{role_name}};
```
#### Grant a set of authorities to a role:
```shell
grant {{action_list}} on {{object_type}} {{object_name}} to role {{role_name}};
```
#### Describe authorities of a role:
```shell
desc role {{role_name}};
```
#### Grant a role to a user:
```shell
grant {{role_name}} to {{username}};
```
{% endraw %}