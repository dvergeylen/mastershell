---
layout: default
title: "piactl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="piactl">
  <a href="/en/common/piactl.html">piactl</a> <a href="#piactl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The command-line tool for Private Internet Access, a commercial VPN provider.
> More information: <https://privateinternetaccess.com/helpdesk/kb/articles/pia-desktop-command-line-interface>.

#### Log in to Private Internet Access:
```shell
piactl login {{path/to/login_file}}
```
#### Connect to Private Internet Access:
```shell
piactl connect
```
#### Disconnect from Private Internet Access:
```shell
piactl disconnect
```
#### Enable or disable the Private Internet Access daemon in the background:
```shell
piactl background {{enable|disable}}
```
#### List all available VPN regions:
```shell
piactl get regions
```
#### Display the current VPN region:
```shell
piactl get region
```
#### Set your VPN region:
```shell
piactl set region {{region}}
```
#### Log out of Private Internet Access:
```shell
piactl logout
```
{% endraw %}