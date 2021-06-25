---
layout: default
title: "docker container"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-container">
  <a href="/ko/common/docker-container.html">docker container</a> <a href="#docker-container"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 도커 컨테이너들을 관리한다.
> 더 많은 정보: <https://docs.docker.com/engine/reference/commandline/container/>.

#### 현재 실행중인 도커 컨테이너들의 목록:
```shell
docker container ls
```
#### 하나 혹은 더 많은 정지된 컨테이너들 실행하기:
```shell
docker container start {{컨테이너1_이름}} {{컨테이너2_이름}}
```
#### 하나 혹은 더 많은 실행중인 컨테이너들 종료하기:
```shell
docker container kill {{컨테이너_이름}}
```
#### 하나 혹은 더 많은 실행중인 컨테이너들 중지하기:
```shell
docker container stop {{컨테이너_이름}}
```
#### 하나 혹은 더 많은 컨테이너들 내에서 모든 프로세스들 일시중지하기:
```shell
docker container pause {{컨테이너_이름}}
```
#### 하나 혹은 더 많은 컨테이너들에 대한 상세 정보 표시하기:
```shell
docker container inspect {{컨테이너_이름}}
```
#### 컨테이너의 파일 시스템을 tar 아카이브로 내보내기:
```shell
docker container export {{컨테이너_이름}}
```
#### 컨테이너의 변경점들로부터 새 이미지 생성하기:
```shell
docker container commit {{컨테이너_이름}}
```
{% endraw %}