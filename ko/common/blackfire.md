---
layout: default
title: "blackfire"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="blackfire">
  <a href="/ko/common/blackfire.html">blackfire</a> <a href="#blackfire"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PHP용 커맨드라인 프로파일링 도구.
> 더 많은 정보: <https://blackfire.io/>.

#### Blackfire 클라이언트 초기화 및 구성:
```shell
blackfire config
```
#### Blackfire agent 시작:
```shell
blackfire agent
```
#### 특정 소켓에서 Blackfire agent 시작:
```shell
blackfire agent --socket="{{tcp://127.0.0.1:8307}}"
```
#### 특정 프로그램에서 프로파일러 실행:
```shell
blackfire run {{파일.php/의/php 경로}}
```
#### 프로파일러 실행 및 샘플 10개 수집:
```shell
blackfire --samples={{10}} run {{파일.php/의/php 경로}}
```
#### 프로파일러 및 출력 결과를 JSON으로 실행:
```shell
blackfire --json run {{파일.php/의/php 경로}}
```
#### 프로파일러 파일을 Blackfire 웹 서비스에 업로드:
```shell
blackfire upload {{파일/의/경로}}
```
#### Blackfire 웹 서비스에서 프로필 상태 확인:
```shell
blackfire status
```
{% endraw %}