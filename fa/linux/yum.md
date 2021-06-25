---
layout: default
title: "yum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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