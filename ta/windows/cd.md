---
layout: default
title: "cd"
date: 2021-06-25 18:12:13 +02:00
---
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
{% endraw %}