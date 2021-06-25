---
layout: default
title: "pio org"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-org">
  <a href="/en/common/pio-org.html">pio org</a> <a href="#pio-org"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage PlatformIO organizations and their owners.
> More information: <https://docs.platformio.org/en/latest/core/userguide/org/>.

#### Create a new organization:
```shell
pio org create {{organization_name}}
```
#### Delete an organization:
```shell
pio org destroy {{organization_name}}
```
#### Add a user to an organization:
```shell
pio org add {{organization_name}} {{username}}
```
#### Remove a user from an organization:
```shell
pio org remove {{organization_name}} {{username}}
```
#### List all organizations the current user is a member of and their owners:
```shell
pio org list
```
#### Update the name, email or display name of an organization:
```shell
pio org update --orgname {{new_organization_name}} --email {{new_email}} --displayname {{new_display_name}} {{organization_name}}
```
{% endraw %}