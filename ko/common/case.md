---
layout: default
title: "case"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="case">
  <a href="/ko/common/case.html">case</a> <a href="#case"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 표현식의 값에 근거하여 분기.
> 더 많은 정보: <https://manned.org/case>.

#### 변수를 문자열 리터럴과 일치시켜 실행할 명령어 결정:
```shell
case {{$tocount}} in {{words}}) {{wc -w README}}; ;; {{lines}}) {{wc -l README}}; ;; esac
```
#### 패턴을 |와 결합하고, *를 대비책 패턴으로 사용:
```shell
case {{$tocount}} in {{[wW]|words}}) {{wc -w README}}; ;; {{[lL]|lines}}) {{wc -l README}}; ;; *) {{echo "what?"}}; ;; esac
```
{% endraw %}