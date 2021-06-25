---
layout: default
title: "balena"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="balena">
  <a href="/ko/common/balena.html">balena</a> <a href="#balena"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 명령 줄에서 balenaCloud, openBalena 및 balena API와 상호 작용하십시오.
> 더 많은 정보: <https://www.balena.io/docs/reference/cli/>.

#### balenaCloud 계정에 로그인:
```shell
balena login
```
#### BalencaCloud 또는 OpenBalena 애플리케이션 생성:
```shell
balena app create {{app_name}}
```
#### 계정 내 모든 balenaCloud 또는 openBalena 애플리케이션 나열:
```shell
balena apps
```
#### balenaCloud 또는 openBalena 계정과 관련된 모든 장치 나열:
```shell
balena devices
```
#### BalenaOS 이미지를 로컬 드라이브에 플래시:
```shell
balena local flash {{path/to/balenaos.img}} --drive {{drive_location}}
```
{% endraw %}