---
layout: default
title: "bup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bup">
  <a href="/ko/common/bup.html">bup</a> <a href="#bup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Git 팩 파일 형식을 기반으로 하는 백업 시스템, 빠른 증분 저장 및. 전역 중복 제거 기능 제공.
> 더 많은 정보: <https://github.com/bup/bup>.

#### 지정된 로컬 디렉토리에서 백업 저장소 초기화:
```shell
bup -d {{저장소/의/경로}} init
```
#### 백업을 수행하기 전에 지정된 디렉토리 준비:
```shell
bup -d {{저장소/의/경로}} index {{디렉토리/의/경로}}
```
#### 저장소에 디렉토리 백업:
```shell
bup -d {{저장소/의/경로}} save -n {{백업명}} {{디렉토리/의/경로}}
```
#### 현재 저장소에 저장된 백업 스냅샷 표시:
```shell
bup -d {{저장소/의/경로}} ls
```
#### 특정 백업 스냅샷을 목적 디렉토리에 복원:
```shell
bup -d {{저장소/의/경로}} restore -C {{타겟_디렉토리/의/경로}} {{백업명}}
```
{% endraw %}