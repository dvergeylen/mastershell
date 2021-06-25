---
layout: default
title: "cordova"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cordova">
  <a href="/ko/common/cordova.html">cordova</a> <a href="#cordova"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> HTML, CSS 및 JS가 포함된 모바일 앱.
> 더 많은 정보: <https://cordova.apache.org/docs/en/latest/guide/cli/>.

#### cordova 프로젝트 생성:
```shell
cordova create {{경로}} {{패키지_명}} {{프로젝트_명}}
```
#### 현재 작업 공간 상태 표시:
```shell
cordova info
```
#### cordova 플랫폼 추가:
```shell
cordova platform add {{플랫폼}}
```
#### cordova 플랫폼 제거:
```shell
cordova platform remove {{플랫폼}}
```
#### cordova 플러그인 추가:
```shell
cordova plugin add {{플러그인id}}
```
#### cordova 플러그인 제거:
```shell
cordova plugin remove {{플러그인id}}
```
{% endraw %}