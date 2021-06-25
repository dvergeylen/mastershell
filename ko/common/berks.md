---
layout: default
title: "berks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="berks">
  <a href="/ko/common/berks.html">berks</a> <a href="#berks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chef 자세한 설명서 의존 관리자.
> 더 많은 정보: <https://docs.chef.io/berkshelf.html>.

#### 로컬 저장소에 자세한 설명서 종속성 설치:
```shell
berks install
```
#### 특정 자세한 설명서와 그 종속성을 업데이트:
```shell
berks update {{자세한 설명서}}
```
#### 자세한 설명서를 Chef server에 업로드:
```shell
berks upload {{자세한 설명서}}
```
#### 자세한 설명서의 종속성 확인:
```shell
berks contingent {{자세한 설명서}}
```
{% endraw %}