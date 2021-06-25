---
layout: default
title: "AdGuardHome"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adguardhome">
  <a href="/ru/common/adguardhome.html">AdGuardHome</a> <a href="#adguardhome"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Программное обеспечение для блокировки рекламы и отслеживания во всей сети.
> Больше информации: <https://github.com/AdguardTeam/AdGuardHome>.

#### Запустить AdGuard Home:
```shell
AdGuardHome
```
#### Запустить AdGuard с заданной конфигурацией:
```shell
AdGuardHome --config {{путь/до/AdGuardHome.yaml}}
```
#### Установить рабочую папку, где будут сохранятья данные:
```shell
AdGuardHome --work-dir {{путь/до/папки}}
```
#### Установить или удалить AdGuard Home как службу:
```shell
AdGuardHome --service {{install|uninstall}}
```
#### Запустить службу AdGuard Home:
```shell
AdGuardHome --service start
```
#### Перезагрузить конфигурацию для службы AdGuard Home:
```shell
AdGuardHome --service reload
```
#### Остановить или перезапустить службу AdGuard Home:
```shell
AdGuardHome --service {{stop|restart}}
```
{% endraw %}