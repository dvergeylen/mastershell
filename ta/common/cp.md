---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/ta/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> கோப்புகளையோ அடைவுகளையோ நகலெடு.
> மேலும் தகவல்: <https://www.gnu.org/software/coreutils/cp>.

#### கோப்பை நகலெடு:
```shell
cp {{மூலக்கோப்பிற்குப்/பாதை}} {{நகல்/கோப்பிற்குப்/பாதை}}
```
#### கோப்பை நகலெடுத்து அடைவொன்றிற்குள் அதே பெயருடன் வை:
```shell
cp {{மூலக்கோப்பிற்குப்/பாதை}} {{நகல்/கோப்பின்/தாயடைவிற்குப்/பாதை}}
```
#### அடைவையும் அதில் உள்ளடங்கிய அனைத்தையும் தற்சுருளாக நகலெடு:
```shell
cp -r {{மூல/அடைவிற்குப்/பாதை}} {{நகல்/அடைவிற்குப்/பாதை}}
```
#### அடைவையும் அதில் உள்ளடங்கிய அனைத்தையும் தற்சுருளாக வளவள நிலையில் (நகலெடுக்கப்படும் கோப்புகள் பட்டியலிடப்படும்) நகலெடு:
```shell
cp -vr {{மூல/அடைவிற்குப்/பாதை}} {{நகல்/அடைவிற்குப்/பாதை}}
```
#### அடைவின் உள்ளடக்கத்தை நகலெடுத்து இன்னொரு அடைவிற்குள் வை:
```shell
cp -r {{மூல/அடைவிற்குப்/பாதை/*}} {{நகல்/அடைவிற்குப்/பாதை}}
```
#### txt வகைப்பெயருடையக் கோப்புகளை ஊடாட்ட நிலையில் (ஏற்கனவே இருக்கும் கோப்புகள் மேலெழுதும் முன் உறுதிப்படுத்தக் கேட்கும்) நகலெடு:
```shell
cp -i {{*.txt}} {{நகல்/அடைவிற்குப்/பாதை}}
```
{% endraw %}