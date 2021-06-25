---
layout: default
title: "balena"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="balena">
  <a href="/en/common/balena.html">balena</a> <a href="#balena"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with the balenaCloud, openBalena and the balena API from the command-line.
> More information: <https://www.balena.io/docs/reference/cli/>.

#### Log in to the balenaCloud account:
```shell
balena login
```
#### Create a balenaCloud or openBalena application:
```shell
balena app create {{app_name}}
```
#### List all balenaCloud or openBalena applications within the account:
```shell
balena apps
```
#### List all devices associated with the balenaCloud or openBalena account:
```shell
balena devices
```
#### Flash a balenaOS image to a local drive:
```shell
balena local flash {{path/to/balenaos.img}} --drive {{drive_location}}
```
{% endraw %}