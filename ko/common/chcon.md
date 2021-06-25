---
layout: default
title: "chcon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chcon">
  <a href="/ko/common/chcon.html">chcon</a> <a href="#chcon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 파일 또는 파일/디렉토리의 SELinux 보안 내용 변경.
> 더 많은 정보: <https://www.gnu.org/software/coreutils/chcon>.

#### 파일의 보안 내용 보기:
```shell
ls -lZ {{경로/파일명}}
```
#### 참조된 파일을 사용하여, 대상 파일의 보안 내용 변경:
```shell
chcon --reference={{참조_파일명}} {{대상_파일명}}
```
#### 파일의 전체 SELinux 보안 내용 변경:
```shell
chcon {{사용자}}:{{역할}}:{{타입}}:{{범위/레벨}} {{파일명}}
```
#### SELinux 보안 내용의 사용자 부분만 변경:
```shell
chcon -u {{사용자}} {{파일명}}
```
#### SELinux 보안 내용의 역할 부분만 변경:
```shell
chcon -r {{역할}} {{파일명}}
```
#### SELinux 보안 컨텍스트의 타입 부분만 변경:
```shell
chcon -t {{타입}} {{파일명}}
```
#### SELinux 보안 컨텍스트의 범위/레벨 부분만 변경:
```shell
chcon -l {{범위/레벨}} {{파일명}}
```
{% endraw %}