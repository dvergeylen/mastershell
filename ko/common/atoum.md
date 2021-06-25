---
layout: default
title: "atoum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atoum">
  <a href="/ko/common/atoum.html">atoum</a> <a href="#atoum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PHP를 위한 단순하고 현대적이며 직관적인 단위 테스트 프레임워크.
> 더 많은 정보: <http://atoum.org>.

#### 설정 파일 초기화:
```shell
atoum --init
```
#### 모든 테스트 실행:
```shell
atoum
```
#### 특정 설정 파일을 사용한 테스트 실행:
```shell
atoum -c {{경로/파일명}}
```
#### 특정 테스트파일 실행:
```shell
atoum -f {{경로/파일명}}
```
#### 특정 테스트 디렉토리 실행:
```shell
atoum -d {{경로/디렉토리명}}
```
#### 특정 namespace 아래 있는 모든 테스트 실행:
```shell
atoum -ns {{namespace}}
```
#### 특정 태그를 갖고 테스트 실행:
```shell
atoum -t {{태그}}
```
#### 테스트를 실행하기 전에 사용자 지정 부트스트랩 파일을 로드:
```shell
atoum --bootstrap-file {{경로/파일명}}
```
{% endraw %}