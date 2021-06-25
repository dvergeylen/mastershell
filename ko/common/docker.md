---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/ko/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 도커 컨테이너들과 이미지들을 관리한다.
> 더 많은 정보: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### 현재 실행중인 도커 컨테이너들 목록보기:
```shell
docker ps
```
#### 모든 도커 컨테이너들(실행중이고 중지된) 목록 보기:
```shell
docker ps -a
```
#### 사용자 정의 이름으로 이미지로부터 컨테이너 실행:
```shell
docker run --name {{컨테이너_이름}} {{이미지}}
```
#### 기존 컨테이너 실행 또는 중지하기:
```shell
docker {{실행|중지}} {{컨테이너_이름}}
```
#### 도커 레지스트리로부터 이미지 가져오기:
```shell
docker pull {{이미지}}
```
#### 이미 실행중인 컨테이너 내부에서 쉘 열기:
```shell
docker exec -it {{컨테이너_이름}} {{쉘}}
```
#### 중지된 컨테이너 제거하기:
```shell
docker rm {{컨테이너_이름}}
```
#### 컨테이너 로그를 가져오고 팔로우하기:
```shell
docker logs -f {{컨테이너_이름}}
```
{% endraw %}