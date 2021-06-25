---
layout: default
title: "docker-machine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-machine">
  <a href="/ko/common/docker-machine.html">docker-machine</a> <a href="#docker-machine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 도커를 실행하는 머신들을 생성하고 관리한다.
> 더 많은 정보: <https://docs.docker.com/machine/reference/>.

#### 현재 실행중인 도커 머신들 목록보기:
```shell
docker-machine ls
```
#### 특정 이름으로 새로운 도커 머신 생성하기:
```shell
docker-machine create {{이름}}
```
#### 머신의 상태 가져오기:
```shell
docker-machine status {{이름}}
```
#### 머신 시작하기:
```shell
docker-machine start {{이름}}
```
#### 머신 중지하기:
```shell
docker-machine stop {{이름}}
```
#### 머신에 대한 정보 검사하기:
```shell
docker-machine inspect {{이름}}
```
{% endraw %}