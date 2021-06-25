---
layout: default
title: "behat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="behat">
  <a href="/ko/common/behat.html">behat</a> <a href="#behat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Behaviour-Driven 개발을 위한 PHP 프레임워크.
> 더 많은 정보: <https://behat.org/>.

#### 새로운 Behat 프로젝트 초기화:
```shell
behat --init
```
#### 모든 테스트 실행:
```shell
behat
```
#### 지정된 suite에서 모든 테스트 실행:
```shell
behat --suite={{suite_명}}
```
#### 특정 출력 formatter로 테스트 실행:
```shell
behat --format {{좋은|진행}}
```
#### 테스트 실행 및 파일로 결과 출력:
```shell
behat --out {{파일/의/경로}}
```
#### 테스트 suite에 정의 목록 표시:
```shell
behat --definitions
```
{% endraw %}