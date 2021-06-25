---
layout: default
title: "browser-sync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="browser-sync">
  <a href="/ko/common/browser-sync.html">browser-sync</a> <a href="#browser-sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일 변경에 따라 브라우저를 업데이트 하는 로컬 웹 서버 시작.
> 더 많은 정보: <https://browsersync.io/docs/command-line>.

#### 특정 디렉토리로부터 서버 시작:
```shell
browser-sync start --server {{디렉토리/의/경로}} --files {{디렉토리/의/경로}}
```
#### 로컬 디렉토리에서 서버 시작, 일부 디렉토리에서 모든 css파일 확인:
```shell
browser-sync start --server --files '{{디렉토리/의/경로/*.css}}'
```
#### 구성 파일 생성:
```shell
browser-sync init
```
#### 구성 파일에서 브라우저 동기화 시작:
```shell
browser-sync start --config {{config_파일}}
```
{% endraw %}