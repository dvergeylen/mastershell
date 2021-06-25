---
layout: default
title: "surge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="surge">
  <a href="/en/common/surge.html">surge</a> <a href="#surge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple command-line web publishing.
> More information: <https://surge.sh>.

#### Upload a new site to surge.sh:
```shell
surge {{path/to/my_project}}
```
#### Deploy site to custom domain (note that the DNS records must point to the surge.sh subdomain):
```shell
surge {{path/to/my_project}} {{my_custom_domain.com}}
```
#### List your surge projects:
```shell
surge list
```
#### Remove a project:
```shell
surge teardown {{my_custom_domain.com}}
```
{% endraw %}