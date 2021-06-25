---
layout: default
title: "composer"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="composer">
  <a href="/ko/common/composer.html">composer</a> <a href="#composer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PHP 프로젝트의 의존성(dependency)을 기반으로 한 매니저 패키지.
> 더 많은 정보: <https://getcomposer.org/>.

#### 프로젝트의 의존성(dependency)으로 패키지를 추가합니다, 다음에 추가합니다 `composer.json`:
```shell
composer require {{사용자/패키지명}}
```
#### 프로젝트의 `composer.json` 안에 모든 의존성(dependency)를 설치합니다 :
```shell
composer install
```
#### 프로젝트의 패키지를 제거하며 `composer.json` 안의 모든 의존성(dependency)를 제거합니다:
```shell
composer remove {{사용자/패키지명}}
```
#### 프로젝트의 `composer.json` 파일의 모든 의존성(dependency)를 업데이트 합니다:
```shell
composer update
```
#### composer를 최신 버전으로 업데이트 합니다:
```shell
composer self-update
```
{% endraw %}