---
layout: default
title: "route"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="route">
  <a href="/en/osx/route.html">route</a> <a href="#route"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manually manipulate the routing tables.
> Necessitates to be root.

#### Add a route to a destination through a gateway:
```shell
sudo route add {{dest_ip_address}} {{gateway_address}}
```
#### Add a route to a /24 subnet through a gateway:
```shell
sudo route add {{subnet_ip_address}}/24 {{gateway_address}}
```
#### Run in test mode (does not do anything, just print):
```shell
sudo route -t add {{dest_ip_address}}/24 {{gateway_address}}
```
#### Remove all routes:
```shell
sudo route flush
```
#### Delete a specific route:
```shell
sudo route delete {{dest_ip_address}}/24
```
#### Lookup and display the route for a destination (hostname or IP address):
```shell
sudo route get {{destination}}
```
{% endraw %}