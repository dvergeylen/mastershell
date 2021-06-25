---
layout: default
title: "touch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="touch">
  <a href="/hi/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> एक फ़ाइल का उपयोग और संशोधन समय (atime, mtime) बदलें।
> अधिक जानकारी: <https://www.gnu.org/software/coreutils/touch>.

#### एक नई खाली फ़ाइल बनाएं (मौजूदा फ़ाइल के लिए समय बदल दें):
```shell
touch {{फ़ाइल का नाम}}
```
#### फ़ाइल को किसी विशिष्ट तिथि और समय पर सेट करें:
```shell
touch -t {{YYYMMDDHHMM.SS}} {{फ़ाइल का नाम}}
```
#### दूसरी फ़ाइल पर समय सेट करने के लिए फ़ाइल से समय का उपयोग करें:
```shell
touch -r {{पहला फ़ाइल का नाम}} {{दूसरा फ़ाइल का नाम}}
```
{% endraw %}