---
layout: default
title: "route"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="route">
  <a href="/en/common/route.html">route</a> <a href="#route"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Use route cmd to set the route table.

#### Display the information of route table:
```shell
route -n
```
#### Add route rule:
```shell
sudo route add -net {{ip_address}} netmask {{netmask_address}} gw {{gw_address}}
```
#### Delete route rule:
```shell
sudo route del -net {{ip_address}} netmask {{netmask_address}} dev {{gw_address}}
```
{% endraw %}