---
layout: default
title: "docker images"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-images">
  <a href="/ko/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 도커 이미지를 관리한다.
> 더 많은 정보: <https://docs.docker.com/engine/reference/commandline/images/>.

#### 모든 도커 이미지 목록보기:
```shell
docker images
```
#### 중간자를 포함한 모든 도커 이미지 목록보기:
```shell
docker images -a
```
#### 잔잔한 모드로 결과 목록보기(수로 표현된 ID들만):
```shell
docker images -q
```
#### 어떠한 컨테이너에서도 사용되지 않은 모든 도커 이미지 목록보기:
```shell
docker images --filter dangling=true
```
{% endraw %}