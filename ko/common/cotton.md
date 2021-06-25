---
layout: default
title: "cotton"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cotton">
  <a href="/ko/common/cotton.html">cotton</a> <a href="#cotton"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 마크다운 테스트 사양 러너.
> 더 많은 정보: <https://github.com/chonla/cotton>.

#### 특정 기본 URL 사용하기:
```shell
cotton -u {{기본_url}} {{파일}}.md
```
#### 인증서 확인 비활성화(비 보안 모드):
```shell
cotton -u {{기본_url}} -i {{파일}}.md
```
#### 테스트 실패시 실행 중지:
```shell
cotton -u {{기본_url}} -s {{파일}}.md
```
{% endraw %}