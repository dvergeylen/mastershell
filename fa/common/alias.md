---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/fa/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ایجاد نام مستعار -- کلمه ای که جایگزین یک دستور می باشد.
> نام های مستعار طول عمری برابر با جلسه جاری شل مربوطه دارند مگر اینکه در فایل های پیکربندی شل مربوط نظیر `~/.bashrc` تعریف شوند.
> اطلاعات بیشتر: <https://tldp.org/LDP/abs/html/aliases.html>.

#### نمایش تمامی نام های مستعار:
```shell
alias
```
#### ایجاد یک نام مستعار:
```shell
alias {{word}}="{{command}}"
```
#### نمایش نام مستعار مرتبط با کلمه مشخص شده:
```shell
alias {{word}}
```
#### حذف یک نام مستعار:
```shell
unalias {{word}}
```
#### تغییر `rm` به نسخه تعاملی با تعریف نام مستعار:
```shell
alias {{rm}}="{{rm -i}}"
```
#### تعریف `la` به عنوان میانبری برای `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}