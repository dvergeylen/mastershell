---
layout: default
title: "chown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chown">
  <a href="/ko/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일과 디렉토리의 사용자 및 그룹 소유권을 변경.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/chown>.

#### 파일/디렉토리의 소유 사용자 변경:
```shell
chown {{사용자}} {{경로/파일명_또는_디렉토리명}}
```
#### 파일/디렉토리의 소유 사용자 및 그룹 변경:
```shell
chown {{사용자}}:{{그룹}} {{경로/파일명_또는_디렉토리명}}
```
#### 디렉토리 소유자와 그 내용을 재귀적으로 변경:
```shell
chown -R {{사용자}} {{경로/디렉토리명}}
```
#### 심볼릭 링크의 소유자 변경:
```shell
chown -h {{사용자}} {{경로/심볼릭_링크}}
```
#### 참조 파일과 일치하도록 파일/디렉토리 소유자 변경:
```shell
chown --reference={{경로/참조_파일명}} {{경로/파일명_또는_디렉토리명}}
```
{% endraw %}