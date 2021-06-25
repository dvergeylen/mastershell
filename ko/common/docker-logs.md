---
layout: default
title: "docker logs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-logs">
  <a href="/ko/common/docker-logs.html">docker logs</a> <a href="#docker-logs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 컨테이너 로그들을 출력한다.
> 더 많은 정보: <https://docs.docker.com/engine/reference/commandline/logs>.

#### 컨테이너로부터 로그들을 출력하기:
```shell
docker logs {{컨테이너_이름}}
```
#### 로그들을 출력하고 추적하기:
```shell
docker logs -f {{컨테이너_이름}}
```
#### 최근 5줄만 출력하기:
```shell
docker logs {{컨테이너_이름}} --tail {{5}}
```
#### 로그들을 출력하고 타임스태프 추가하기:
```shell
docker logs -t {{컨테이너_이름}}
```
#### 특정 시점의 컨테이너 실행 시점으로부터 로그 출력하기 (예시. 23m, 10s, 2013-01-02T13:23:37):
```shell
docker logs {{컨테이너_이름}} --until {{시간}}
```
{% endraw %}