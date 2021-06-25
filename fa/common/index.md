---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#alias">alias</a>
* <a href="#cat">cat</a>
* <a href="#cd">cd</a>
* <a href="#cp">cp</a>
* <a href="#false">false</a>
* <a href="#fg">fg</a>
* <a href="#logname">logname</a>
* <a href="#ls">ls</a>
* <a href="#nohup">nohup</a>
* <a href="#sleep">sleep</a>
* <a href="#time">time</a>
* <a href="#tty">tty</a>
* <a href="#uname">uname</a>
* <a href="#unclutter">unclutter</a>
* <a href="#users">users</a>
* <a href="#view">view</a>

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
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/fa/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> تغییر دایرکتوری جاری.
> اطلاعات بیشتر: <https://man.archlinux.org/man/cd.n>.

#### تغییر مسیربه دایرکتوری مشخص شده:
```shell
cd {{path/to/directory}}
```
#### تغییر مسیر به دایرکتوری Home کاربر فعلی:
```shell
cd
```
#### تغییر مسیر به دایرکتوری بالاتر از مسیر جاری:
```shell
cd ..
```
#### تغییر مسیر به دایرکتوری قبلی:
```shell
cd -
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="false">
  <a href="/fa/common/false.html">false</a> <a href="#false"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> برگرداندن 1 به عنوان کد خروجی.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/false>.

#### برگرداندن 1 به عنوان کد خروجی:
```shell
false
```
{% endraw %}{% raw %}
<h2 id="fg">
  <a href="/fa/common/fg.html">fg</a> <a href="#fg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> اجرای کارها در پیش زمینه.
> اطلاعات بیشتر: <https://manned.org/fg>.

#### آوردن آخرین کار اجرا شده در پس زمینه به پیش زمینه:
```shell
fg
```
#### آوردن کار با آی دی مشخص شده به پیش زمینه:
```shell
fg %{{job_id}}
```
{% endraw %}{% raw %}
<h2 id="logname">
  <a href="/fa/common/logname.html">logname</a> <a href="#logname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نمایش نام کاربر.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/logname>.

#### نمایش نام کاربر لاگین شده:
```shell
logname
```
{% endraw %}{% raw %}
<h2 id="ls">
  <a href="/fa/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نمایش محتویات دایرکتوری.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/ls>.

#### نمایش فایل ها به صورت خطی:
```shell
ls -1
```
#### نمایش کلیه فایل ها، شامل فایل های مخفی:
```shell
ls -a
```
#### نمایش فایل ها، با این تفاوت که / به نام دایرکتوری ها اضافه می شود:
```shell
ls -F
```
#### نمایش فایل ها به همراه مجوزها، مالک، اندازه و تاریخ تغییرات:
```shell
ls -la
```
#### نمایش فایل ها به همراه مجوزها، مالک، اندازه و تاریخ تغییرات، اندازه ها به صورت قابل درک برای انسان:
```shell
ls -lh
```
#### نمایش فایل ها به همراه مجوزها، مالک، اندازه و تاریخ تغییرات، مرتب شده با اندازه فایل به صورت نزولی:
```shell
ls -lS
```
#### نمایش فایل ها به همراه مجوزها، مالک، اندازه و تاریخ تغییرات، مرتب شده با تاریخ تغییر فایل به صورت صعودی:
```shell
ls -ltr
```
{% endraw %}{% raw %}
<h2 id="nohup">
  <a href="/fa/common/nohup.html">nohup</a> <a href="#nohup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> اجرای یک پردازش در پس زمینه حتی زمانی که ترمینال بسته شود.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/nohup>.

#### اجرای پردازش در پس زمینه فارغ از اجرا بودن ترمینال:
```shell
nohup {{command}} {{command_options}}
```
{% endraw %}{% raw %}
<h2 id="sleep">
  <a href="/fa/common/sleep.html">sleep</a> <a href="#sleep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ایجاد تاخیر بر اساس زمان.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/sleep>.

#### تاخیر به ثانیه:
```shell
sleep {{seconds}}
```
#### تاخیر به دقیقه:
```shell
sleep {{minutes}}m
```
#### تاخیر به ساعت:
```shell
sleep {{hours}}h
```
{% endraw %}{% raw %}
<h2 id="time">
  <a href="/fa/common/time.html">time</a> <a href="#time"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نمایش زمان اجرای یک دستور.

#### نمایش زمان اجرای دستور `ls`:
```shell
time ls
```
{% endraw %}{% raw %}
<h2 id="tty">
  <a href="/fa/common/tty.html">tty</a> <a href="#tty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نمایش نام ترمینال.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/tty>.

#### نمایش نام فایل ترمینال جاری:
```shell
tty
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="unclutter">
  <a href="/fa/common/unclutter.html">unclutter</a> <a href="#unclutter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> مخفی کردن نشان ماوس.

#### مخفی کردن نشان ماوس بعد از 3 ثانیه:
```shell
unclutter -idle {{3}}
```
{% endraw %}{% raw %}
<h2 id="users">
  <a href="/fa/common/users.html">users</a> <a href="#users"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نمایش لیست کاربران لاگین شده.
> اطلاعات بیشتر: <https://www.gnu.org/software/coreutils/users>.

#### نمایش لیست کاربران لاگین شده:
```shell
users
```
#### نمایش لیست کاربران لاگین شده بر اساس یک لاگ فایل خاص:
```shell
users {{/var/log/wmtp}}
```
{% endraw %}{% raw %}
<h2 id="view">
  <a href="/fa/common/view.html">view</a> <a href="#view"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> نسخه فقط خواندنی vim.
> معادل vim -R.

#### باز کردن فایل:
```shell
view {{file}}
```
{% endraw %}