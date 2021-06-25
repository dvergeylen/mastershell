---
layout: default
title: "bitcoin-cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bitcoin-cli">
  <a href="/ko/common/bitcoin-cli.html">bitcoin-cli</a> <a href="#bitcoin-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> RPC 호출을 통해 비트코인 데몬과 상호 작용하는 커맨드라인 클라이언트.`bitcoin.conf`에 정의된 구성 사용.
> 더 많은 정보:<https://en.bitcoin.it/wiki/Running_Bitcoin#Command-line_arguments>.

#### 지정된 주소로 트랜잭션 전송:
```shell
bitcoin-cli sendtoaddress "{{주소}}" {{양}}
```
#### 하나 이상의 블록 생성:
```shell
bitcoin-cli generate {{블록_갯수}}
```
#### wallet에 대한 고급 정보 출력:
```shell
bitcoin-cli getwalletinfo
```
#### 보내지지 않은 모든 트랜잭션의 출력 나열:
```shell
bitcoin-cli listunspent
```
#### wallet 정보를 텍스트 파일로 출력:
```shell
bitcoin-cli dumpwallet "{{파일/의/경로}}"
```
{% endraw %}