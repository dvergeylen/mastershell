---
layout: default
title: "cargo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cargo">
  <a href="/ko/common/cargo.html">cargo</a> <a href="#cargo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rust 패키지 관리프로그램.
> Rust 프로젝트 및 해당 모듈 종속성(크레이트) 관리.
> 더 많은 정보: <https://crates.io/>.

#### 크레이트 검색:
```shell
cargo search {{검색할_문자열}}
```
#### 크레이트 설치:
```shell
cargo install {{크레이트_이름}}
```
#### 설치된 크레이트 목록:
```shell
cargo install --list
```
#### 현재 디렉토리에 새 이진 또는 라이브러리 Rust 프로젝트 생성:
```shell
cargo init --{{bin|lib}}
```
#### 지정된 디렉토리에 새 이진 또는 라이브러리 Rust 프로젝트 생성:
```shell
cargo new {{경로/디렉토리}} --{{bin|lib}}
```
#### 현재 디렉토리에 Rust 프로젝트 구축:
```shell
cargo build
```
#### 특정 쓰레드 수를 사용하여 구축(기본값은 CPU 코어 수):
```shell
cargo build -j {{작업}}
```
{% endraw %}