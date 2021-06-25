---
layout: default
title: "bash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bash">
  <a href="/ko/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell. `sh`-호환 명령 행 인터프리터.
> 더 많은 정보: <https://gnu.org/software/bash>.

#### 대화식 쉘 시작:
```shell
bash
```
#### 명령 실행:
```shell
bash -c "{{command}}"
```
#### 파일에서 명령 실행:
```shell
bash {{file.sh}}
```
#### 파일에서 명령 실행하고, 터미널에서 실행 된 모든 명령 기록:
```shell
bash -x {{file.sh}}
```
#### 파일에서 명령 실행하고, 첫 번째 에러에서 중지:
```shell
bash -e {{file.sh}}
```
#### stdin에서 명령 실행:
```shell
bash -s
```
#### bash의 버전 정보 출력 (`echo $BASH_VERSION`을 사용하여 버전 문자열만 표시):
```shell
bash --version
```
{% endraw %}