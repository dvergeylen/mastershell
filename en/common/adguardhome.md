---
layout: default
title: "AdGuardHome"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adguardhome">
  <a href="/en/common/adguardhome.html">AdGuardHome</a> <a href="#adguardhome"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A network-wide software for blocking ads & tracking.
> More information: <https://github.com/AdguardTeam/AdGuardHome>.

#### Run AdGuard Home:
```shell
AdGuardHome
```
#### Run AdGuard Home with a specific config:
```shell
AdGuardHome --config {{path/to/AdGuardHome.yaml}}
```
#### Set the work directory for data to be stored in:
```shell
AdGuardHome --work-dir {{path/to/directory}}
```
#### Install or uninstall AdGuard Home as a service:
```shell
AdGuardHome --service {{install|uninstall}}
```
#### Start the AdGuard Home service:
```shell
AdGuardHome --service start
```
#### Reload the configuration for the AdGuard Home service:
```shell
AdGuardHome --service reload
```
#### Stop or restart the AdGuard Home service:
```shell
AdGuardHome --service {{stop|restart}}
```
{% endraw %}