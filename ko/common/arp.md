---
layout: default
title: "arp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp">
  <a href="/ko/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 시스템의 ARP 캐시 표시 및 조작.
> 더 많은 정보: <https://manned.org/arp>.

#### 현재 arp 테이블을 보여줍니다:
```shell
arp -a
```
#### 전체 캐시 삭제:
```shell
sudo arp -a -d
```
#### 특정 엔트리 삭제:
```shell
arp -d {{address}}
```
#### 엔트리 생성:
```shell
arp -s {{address}} {{mac_address}}
```
{% endraw %}