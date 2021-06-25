---
layout: default
title: "df"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="df">
  <a href="/ko/common/df.html">df</a> <a href="#df"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일 시스템 디스크 공간 사용량에 대한 개요를 제공합니다.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/df>.

#### 모든 파일 시스템들과 그들의 디스크 사용량 출력:
```shell
df
```
#### 사람이 읽을 수 있는 형태로 모든 파일시스템들과 그들의 디스크 사용량 출력:
```shell
df -h
```
#### 주어진 파일이나 디렉토리를 포함하는 파일 시스템과 그것의 디스크 사용량 출력:
```shell
df {{경로/파일_혹은_디렉토리명}}
```
#### 사용 가능한 inode들의 수에 대한 통계 출력:
```shell
df -i
```
{% endraw %}