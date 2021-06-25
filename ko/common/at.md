---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/ko/common/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 명령 실행 후 한 번 실행합니다.
> 서비스 AD(또는 ATRUN)는 실제 실행을 위해 실행되어야 합니다.
> 더 많은 정보: <https://man.archlinux.org/man/at.1>.

#### 표준 입력에서 명령을 5분 내에 실행(작업이 끝나면 `Ctrl + D` 를 누르세요):
```shell
at now + 5 minutes
```
#### 오전 10시에 표준 입력에서 명령을 실행하십시오:
```shell
echo "{{./make_db_backup.sh}}" | at 1000
```
#### 다음 주 화요일에 주어진 파일에서 명령을 실행하십시오:
```shell
at -f {{경로/파일명}} 9:30 PM Tue
```
{% endraw %}