---
layout: default
title: "docker-compose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-compose">
  <a href="/ko/common/docker-compose.html">docker-compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 다중 도커 응용 프로그램 실행 및 관리합니다.
> 더 많은 정보: <https://docs.docker.com/compose/reference/overview/>.

#### 실행 중인 모든 컨테이너들 목록:
```shell
docker-compose ps
```
#### 현재 디렉토리로로부터 `docker-compose.yml` 파일을 사용하여 백그라운드에서 모든 컨테이너들을 생성하고 실행하기:
```shell
docker-compose up -d
```
#### 모든 컨테이너들을 실행하고, 필요 시 재조립:
```shell
docker-compose up --build
```
#### 대체 구성 파일을 사용하여 모든 컨테이너들 실행하기:
```shell
docker-compose --file {{경로/파일명}} up
```
#### 실행중인 모든 컨테이너들 중지하기:
```shell
docker-compose stop
```
#### 모든 컨테이너들, 네트워크, 이미지, 그리고 볼륨을 중지하고 제거하기:
```shell
docker-compose down --rmi all --volumes
```
#### 모든 컨테이너들에 대한 로그들 팔로우:
```shell
docker-compose logs --follow
```
{% endraw %}