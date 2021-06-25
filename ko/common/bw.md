---
layout: default
title: "bw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bw">
  <a href="/ko/common/bw.html">bw</a> <a href="#bw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bitwarden 보관함에 접속과 관리를 위한 CLI.
> 더 많은 정보: <https://help.bitwarden.com/article/cli/>.

#### Bitwarden 사용자 계정 로그인:
```shell
bw login
```
#### 사용자 계정 로그아웃:
```shell
bw logout
```
#### Bitwarden 보관함으로부터 아이템 검색과 출력:
```shell
bw list items --search {{github}}
```
#### Bitwarden 보관함으로부터 특정 아이템 출력:
```shell
bw get item {{github}}
```
#### Bitwarden 보관함에 폴더 생성:
```shell
{{echo -n '{"name":"My Folder1"}' | base64}} | bw create folder
```
{% endraw %}