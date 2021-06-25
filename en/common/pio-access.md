---
layout: default
title: "pio access"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-access">
  <a href="/en/common/pio-access.html">pio access</a> <a href="#pio-access"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the access level on published resources (packages) in the registry.
> More information: <https://docs.platformio.org/en/latest/core/userguide/access/>.

#### Grant a user access to a resource:
```shell
pio access grant {{guest|maintainer|admin}} {{username}} {{resource_urn}}
```
#### Remove a user's access to a resource:
```shell
pio access revoke {{username}} {{resource_urn}}
```
#### Show all resources that a user or team has access to and the access level:
```shell
pio access list {{username}}
```
#### Restrict access to a resource to specific users or team members:
```shell
pio access private {{resource_urn}}
```
#### Allow all users access to a resource:
```shell
pio access public {{resource_urn}}
```
{% endraw %}