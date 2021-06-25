---
layout: default
title: "ab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ab">
  <a href="/ta/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> அப்பாச்சி தரப்படுத்தல் கருவி. சுமை சோதனை செய்ய எளிய கருவி.
> மேலும் தகவல்: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### கொடுக்கப்பட்ட முகவரி க்கு 100 HTTP GET கோரிக்கைகளை இயக்கவும்:
```shell
ab -n {{100}} {{முகவரி}}
```
#### கொடுக்கப்பட்ட முகவரி க்கு 100 HTTP GET கோரிக்கைகளை ஒரே நேரத்தில் 10 கோரிக்கைகள் வீதம் செயல்படுத்தவும் :
```shell
ab -n {{100}} -c {{10}} {{முகவரி}}
```
#### இணைப்பை தொடரச்செய்:
```shell
ab -k {{முகவரி}}
```
#### தரப்படுத்தல் குறிக்க செலவழிக்க அதிகபட்ச விநாடிகளை அமைக்கவும்:
```shell
ab -t {{60}} {{முகவரி}}
```
{% endraw %}