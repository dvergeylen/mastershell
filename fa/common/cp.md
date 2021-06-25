---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/fa/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> کپی فایل ها و دایرکتوری ها.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/cp>.

#### کپی فایل از مبدا به مقصد مشخص شده:
```shell
cp {{path/to/source_file.ext}} {{path/to/target_file.ext}}
```
#### کپی فایل به دایرکتوری مشخص شده با حفظ نام فایل:
```shell
cp {{path/to/source_file.ext}} {{path/to/target_parent_directory}}
```
#### کپی یک دایرکتوری به صورت کامل به مقصد جدید(اگر در مقصد دایرکتوری وجود داشت دایرکتوری مبدا در داخل دایرکتوری مقصد کپی می شود):
```shell
cp -R {{path/to/source_directory}} {{path/to/target_directory}}
```
#### کپی یک دایرکتوری به صورت کامل با نمایش جزییات (نمایش فایل های کپی شده):
```shell
cp -vR {{path/to/source_directory}} {{path/to/target_directory}}
```
#### کپی کلیه فایل های با پسوند `txt` به دایرکتوری مقصد در حالت تعاملی (قبل از بازنویسی تاییده توسط کاربر نیاز است):
```shell
cp -i {{*.txt}} {{path/to/target_directory}}
```
#### کپی لینک به مقصد بدون ارجاع به فایل اصلی:
```shell
cp -L {{link}} {{path/to/target_directory}}
```
{% endraw %}