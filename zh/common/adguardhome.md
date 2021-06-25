---
layout: default
title: "AdGuardHome"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adguardhome">
  <a href="/zh/common/adguardhome.html">AdGuardHome</a> <a href="#adguardhome"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一款全网广告拦截与反跟踪软件.
> 更多信息: <https://github.com/AdguardTeam/AdGuardHome>.

#### 运行 AdGuard Home:
```shell
AdGuardHome
```
#### 使用给定的配置文件运行 AdGuard Home:
```shell
AdGuardHome --config {{给定的/配置文件.yaml}}
```
#### 设置存储数据的工作目录:
```shell
AdGuardHome --work-dir {{工作目录/路径}}
```
#### 安装或卸载 AdGuard Home 的服务:
```shell
AdGuardHome --service {{install|uninstall}}
```
#### 启动 AdGuard Home 的服务:
```shell
AdGuardHome --service start
```
#### 刷新 AdGuard Home 服务的设置项:
```shell
AdGuardHome --service reload
```
#### 停止或重启 AdGuard Home 的服务:
```shell
AdGuardHome --service {{stop|restart}}
```
{% endraw %}