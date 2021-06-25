---
layout: default
title: "knife"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="knife">
  <a href="/en/common/knife.html">knife</a> <a href="#knife"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for interacting with a Chef server from a local Chef repo.
> More information: <https://docs.chef.io/knife.html>.

#### Bootstrap a new node:
```shell
knife bootstrap {{fqdn_or_ip}}
```
#### List all registered nodes:
```shell
knife node list
```
#### Show a node:
```shell
knife node show {{node_name}}
```
#### Edit a node:
```shell
knife node edit {{node_name}}
```
#### Edit a role:
```shell
knife role edit {{role_name}}
```
#### View a data bag:
```shell
knife data bag show {{data_bag_name}} {{data_bag_item}}
```
#### Upload a local cookbook to the Chef server:
```shell
knife cookbook upload {{cookbook_name}}
```
{% endraw %}