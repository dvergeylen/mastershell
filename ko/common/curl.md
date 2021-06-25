---
layout: default
title: "curl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="curl">
  <a href="/ko/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 데이터를 서버에서 혹은 서버로 전송.
> HTTP,FTP 및 POP3를 포함한 대부분의 프로토콜 지원.
> 더 많은 정보: <https://curl.se>.

#### URL의 내용을 파일로 다운로드:
```shell
curl {{http://example.com}} --output {{파일명}}
```
#### URL에 표시된 파일 명으로 출력을 저장하고 파일을 다운로드:
```shell
curl --remote-name {{http://example.com/filename}}
```
#### [L]위치 리다이렉션 후 파일을 다운로드 하고, 자동으로 이전 파일 [C]전송(재시작):
```shell
curl --remote-name --location --continue-at - {{http://example.com/filename}}
```
#### 양식 인코딩 데이터 전송(`application/x-www-form-urlencoded`유형의 POST 요청):
```shell
curl --data {{'name=bob'}} {{http://example.com/form}}
```
#### 사용자 지정 HTTP 메서드를 사용하여 추가 헤더로 요청 전송:
```shell
curl --header {{'X-My-Header: 123'}} --request {{PUT}} {{http://example.com}}
```
#### 적절한 컨텐츠 유형 헤더를 지정하여 JSON 포멧으로 데이터 전송:
```shell
curl --data {{'{"name":"bob"}'}} --header {{'Content-Type: application/json'}} {{http://example.com/users/123}}
```
#### 서버 인증을 위한 사용자 이름 및 비밀번호 전달:
```shell
curl --user myusername:mypassword {{http://example.com}}
```
#### 리소스에 대한 클라이언트 인증서 및 키 전달, 인증서 유효성 검사 스킵:
```shell
curl --cert {{클라이언트.pem}} --key {{키.pem}} --insecure {{https://example.com}}
```
{% endraw %}