---
layout: default
title: "conda"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="conda">
  <a href="/ko/common/conda.html">conda</a> <a href="#conda"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 프로그래밍 언어에 대한 패키지, 의존성 및 환경 관리.
> 더 많은 정보: <https://github.com/conda/conda>.

#### 새로운 환경을 생성합니다, 이름이 주어진 패키지로 설치합니다:
```shell
conda create --name {{환경_이름}} {{python=2.7 matplotlib}}
```
#### 모든 환경의 리스트를 보여줍니다:
```shell
conda info --envs
```
#### 환경을 불러오거나 내립니다:
```shell
conda {{활성화|비활성화}} {{환경_이름}}
```
#### 모든 환경을 제거합니다 (모든 패키지 제거):
```shell
conda remove --name {{환경_이름}} --all
```
#### 패키지 이름으로 conda의 채널을 찾습니다:
```shell
conda search {{패키지명}}
```
#### 현재 환경의 패키지를 설치합니다:
```shell
conda install {{python=3.4 numpy}}
```
#### 현재 혼경의 설치된 패키지의 리스트를 보여줍니다:
```shell
conda list
```
#### 사용하지 않는 패키지나 캐시를 제거합니다:
```shell
conda clean --all
```
{% endraw %}