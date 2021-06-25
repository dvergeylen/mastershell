---
layout: default
title: "avrdude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="avrdude">
  <a href="/ko/common/avrdude.html">avrdude</a> <a href="#avrdude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Atmel AVR 마이크로 컨트롤러 프로그래밍을 위한 드라이버 프로그램.
> 더 많은 정보: <https://www.nongnu.org/avrdude/>.

#### AVR 마이크로 컨트롤러 읽기:
```shell
avrdude -p {{AVR_device}} -c {{programmer}} -U flash:r:{{file.hex}}:i
```
#### AVR 마이크로 컨트롤러 쓰기:
```shell
avrdude -p {{AVR_device}} -c {{programmer}} -U flash:w:{{file.hex}}
```
#### 사용 가능한 AVR 장치 목록:
```shell
avrdude -p \?
```
#### 사용 가능한 AVR 프로그래머 목록:
```shell
avrdude -c \?
```
{% endraw %}