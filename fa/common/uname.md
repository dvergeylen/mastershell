---
layout: default
title: "uname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uname">
  <a href="/fa/common/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نمایش اطلاعاتی درباره سخت افزار و سیستم عامل.
> نکته: برای دستیابی به اطلاعات اضافه در رابطه با سیستم عامل از دستور `lsb_release` استفاده کنید.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/uname>.

#### نمایش اطلاعات مربوط به سخت افزار و پردازنده سیستم:
```shell
uname -mp
```
#### نمایش اطلاعات مربوط به نرم افزار از جمله: سیستم عامل، شماره انتشار و نسخه:
```shell
uname -srv
```
#### نمایش نام سیستم:
```shell
uname -n
```
#### نمایش تمامی اطلاعات سیستم(سخت افزار، نرم افزار، نام سیستم):
```shell
uname -a
```
{% endraw %}