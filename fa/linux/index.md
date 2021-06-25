---
layout: default
title: "linux"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#whatis">whatis</a>
* <a href="#whereis">whereis</a>
* <a href="#yum">yum</a>

{% raw %}
<h2 id="whatis">
  <a href="/fa/linux/whatis.html">whatis</a> <a href="#whatis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نمایش توضیحات یک خطی از صفحات راهنما.

#### نمایش توضیحات یک دستور از صفحات راهنما:
```shell
whatis {{command}}
```
#### توضیحات در آخر خط ترمینال برش نمی خورد:
```shell
whatis --long {{command}}
```
#### نمایش توضیحات تمامی دستورات مطابق با الگو:
```shell
whatis --wildcard {{net*}}
```
#### جستجو در توضیحات صفحات راهنما با عبارات منظم:
```shell
whatis --regex '{{wish[0-9]\.[0-9]}}'
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="yum">
  <a href="/fa/linux/yum.html">yum</a> <a href="#yum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ابزار مدیریت بسته برای ردهت، فدورا و سنت اواس(برای نسخه های قدیمی).
> اطلاعات بیشتر: <https://man7.org/linux/man-pages/man8/yum.8.html>.

#### نصب یک بسته:
```shell
yum install {{package}}
```
#### نصب یک بسته با فرض بر اینکه پاسخ شما برای تمامی سوالات بله است(با گزینه update هم می توان از این روش استفاده کرد، مناسب برای به روز رسانی خودکار):
```shell
yum -y install {{package}}
```
#### پیدا کردن بسته ای که دستور مورد نظر را فراهم می کند:
```shell
yum provides {{command}}
```
#### حذف یک بسته:
```shell
yum remove {{package}}
```
#### نمایش به روز رسانی ها برای بسته های نصب شده:
```shell
yum check-update
```
#### به روز رسانی بسته های نصب شده به آخرین نسخه موجود:
```shell
yum upgrade
```
{% endraw %}