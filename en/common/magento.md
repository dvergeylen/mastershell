---
layout: default
title: "magento"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="magento">
  <a href="/en/common/magento.html">magento</a> <a href="#magento"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI for managing the Magento PHP framework.
> More information: <https://magento.com>.

#### Enable one or more space-separated modules:
```shell
magento module:enable {{module(s)}}
```
#### Disable one or more space-separated modules:
```shell
magento module:disable {{module(s)}}
```
#### Update the database after enabling modules:
```shell
magento setup:upgrade
```
#### Update code and dependency injection configuration:
```shell
magento setup:di:compile
```
#### Deploy static assets:
```shell
magento setup:static-content:deploy
```
#### Enable maintenance mode:
```shell
magento maintenance:enable
```
#### Disable maintenance mode:
```shell
magento maintenance:disable
```
#### List all available commands:
```shell
magento list
```
{% endraw %}