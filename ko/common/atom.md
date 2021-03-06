---
layout: default
title: "atom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atom">
  <a href="/ko/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 플러그 기능이 있는 교차 플랫폼 텍스트 편집기.
> 플러그는 `apm`에 의해 관리됩니다.
> 더 많은 정보: <https://atom.io/>.

#### 파일이나 디렉토리 열기:
```shell
atom {{경로/파일명_또는_디렉토리명}}
```
#### 새로운 창에서 파일이나 디렉토리 열기:
```shell
atom -n {{경로/파일명_또는_디렉토리명}}
```
#### 현재 창에서 파일이나 디렉토리 열기:
```shell
atom --add {{경로/파일명_또는_디렉토리명}}
```
#### 안전모드에서 atom 열기Open atom in safe mode (추가 패키지를 로드하지 마시오):
```shell
atom --safe
```
#### 백그라운드에서 fork하지 않도록 막기, atom을 터미널에 부착합니다:
```shell
atom --foreground
```
{% endraw %}