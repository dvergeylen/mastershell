---
layout: default
title: "cryfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cryfs">
  <a href="/ko/common/cryfs.html">cryfs</a> <a href="#cryfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 클라우드용 암호화 파일 시스템.
> 더 많은 정보: <https://www.cryfs.org/>.

#### 암호화 된 파일 시스템 마운트. 초기화 마법사는 처음 실행될 때 시작:
```shell
cryfs {{cipher_dir/의/경로}} {{마운트_포인트/의/경로}}
```
#### 암호화 된 파일 시스템 마운트 해제:
```shell
cryfs-unmount {{마운트_포인트/의/경로}}
```
#### 10분 동안 활동이 없으면 자동으로 마운트 해제:
```shell
cryfs --unmount-idle {{10}} {{cipher_dir/의/경로}} {{마운트_포인트/의/경로}}
```
#### 지원되는 암호 목록 표시:
```shell
cryfs --show-ciphers
```
{% endraw %}