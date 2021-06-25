---
layout: default
title: "windows"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#cd">cd</a>
* <a href="#cls">cls</a>
* <a href="#cmd">cmd</a>

{% raw %}
<h2 id="cd">
  <a href="/ta/windows/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> தற்போதைய பணி அடைவின் பெயரைக் காட்டுகிறது அல்லது மாற்றுகிறது.
> மேலும் தகவல்: <https://docs.microsoft.com/windows-server/administration/windows-commands/cd>.

#### அதே இயக்ககத்தில் ஒரு கோப்பகத்திற்குச் செல்லவும்:
```shell
cd {{கோப்பகத்திற்கான/பாதை}}
```
#### தற்போதைய கோப்பகத்தின் பெயரைக் காண்பி:
```shell
cd
```
#### தற்போதைய கோப்பகத்தின் பெற்றோர் வரை செல்லுங்கள்:
```shell
cd ..
```
#### வேறு இயக்ககத்தில் ஒரு கோப்பகத்திற்குச் செல்லவும்:
```shell
cd {{கோப்பகத்திற்கான/பாதை}} /d
```
{% endraw %}{% raw %}
<h2 id="cls">
  <a href="/ta/windows/cls.html">cls</a> <a href="#cls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> திரையை அழிக்கிறது.
> மேலும் தகவல்: <https://docs.microsoft.com/windows-server/administration/windows-commands/cls>.

#### திரையை அழிக்கவும்:
```shell
cls
```
{% endraw %}{% raw %}
<h2 id="cmd">
  <a href="/ta/windows/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> விண்டோஸ் கட்டளை மொழிபெயர்ப்பாளர்.
> மேலும் தகவல்: <https://docs.microsoft.com/windows-server/administration/windows-commands/cmd>.

#### கட்டளை மொழிபெயர்ப்பாளரின் புதிய நிகழ்வைத் தொடங்கவும்:
```shell
cmd
```
#### குறிப்பிட்ட கட்டளையை இயக்கவும், பின்னர் வெளியேறவும்:
```shell
cmd /c "{{கட்டளை}}"
```
#### குறிப்பிட்ட கட்டளையை இயக்கவும், பின்னர் ஒரு ஊடாடும் ஷெல்லை உள்ளிடவும்:
```shell
cmd /k "{{கட்டளை}}"
```
#### கட்டளை வெளியீட்டில் `echo` இன் பயன்பாட்டை முடக்கு:
```shell
cmd /q
```
#### கட்டளை நீட்டிப்புகளை இயக்கவும் அல்லது முடக்கவும்:
```shell
cmd /e:{{on|off}}
```
#### கோப்பு அல்லது கோப்பக தானியங்குநிரலை இயக்கவும் அல்லது முடக்கவும்:
```shell
cmd /f:{{on|off}}
```
#### சூழல் மாறி விரிவாக்கத்தை இயக்கவும் அல்லது முடக்கவும்:
```shell
cmd /v:{{on|off}}
```
#### யூனிகோட் குறியாக்கத்தைப் பயன்படுத்த வெளியீட்டை கட்டாயப்படுத்தவும்:
```shell
cmd /u
```
{% endraw %}