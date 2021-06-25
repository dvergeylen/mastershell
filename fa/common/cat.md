---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/fa/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> چاپ و ترکیب کردن فایل ها.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/cat>.

#### چاپ محتویات فایل بر روی صفحه نمایش:
```shell
cat {{file}}
```
#### ادغام چند فایل با هم و ایجاد فایل جدید:
```shell
cat {{file1}} {{file2}} > {{target_file}}
```
#### ادغام چند فایل با هم و اضافه کردن آن به فایل مقصد:
```shell
cat {{file1}} {{file2}} >> {{target_file}}
```
#### شمارش تعداد خط های فایل:
```shell
cat -n {{file}}
```
#### نمایش محتویات فایل بدون فضای خالی (نا مناسب برای چاپ):
```shell
cat -v -t -e {{file}}
```
{% endraw %}