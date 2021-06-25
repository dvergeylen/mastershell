---
layout: default
title: "whereis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whereis">
  <a href="/fa/linux/whereis.html">whereis</a> <a href="#whereis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> پیداکردن فایل اجرایی، سورس، صفحه راهنما برای یک دستور.

#### پیداکردن فایل اجرایی، سورس و صفحه راهنما برای ssh:
```shell
whereis {{ssh}}
```
#### پیداکردن فایل اجرایی و صفحه راهنما برای ls:
```shell
whereis -bm {{ls}}
```
#### پیداکردن سورس برای gcc و صفحه راهنما برای git:
```shell
whereis -s {{gcc}} -m {{git}}
```
#### پیداکردن فایل اجرایی برای gcc در مسیر `/usr/bin/`:
```shell
whereis -b -B {{/usr/bin/}} -f {{gcc}}
```
#### پیدا کردن فایل های اجرایی غیر عادی(برای آنهایی که بیشتر از یک فایل اجرایی در سیستم دارند):
```shell
whereis -u *
```
#### پیدا کردن صفحات راهنمای غیر عادی(برای آنهایی که بیشتر از یک فایل اجرایی در سیستم دارند):
```shell
whereis -u -m *
```
{% endraw %}