---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#cat">cat</a>
* <a href="#cd">cd</a>
* <a href="#chsh">chsh</a>
* <a href="#false">false</a>
* <a href="#git-init">git init</a>
* <a href="#ls">ls</a>
* <a href="#mkdir">mkdir</a>
* <a href="#time">time</a>
* <a href="#tldr">tldr</a>
* <a href="#touch">touch</a>
* <a href="#view">view</a>

{% raw %}
<h2 id="cat">
  <a href="/hi/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> फ़ाइलों को प्रिंट और संक्षिप्त करें।
> अधिक जानकारी: <https://www.gnu.org/software/coreutils/cat>.

#### मानक आउटपुट में फ़ाइल की सामग्री प्रिंट करें:
```shell
cat {{फ़ाइल}}
```
#### लक्ष्य फ़ाइल में कई फ़ाइलों को संयुक्त करें:
```shell
cat {{फ़ाइल1}} {{फ़ाइल2}} > {{लक्ष्य_फ़ाइल}}
```
#### लक्ष्य फ़ाइल के अंत में कई फ़ाइलें संलग्न करें:
```shell
cat {{फ़ाइल1}} {{फ़ाइल2}} >> {{लक्ष्य_फ़ाइल}}
```
#### सभी आउटपुट लाइनों की संख्या:
```shell
cat -n {{फ़ाइल}}
```
#### गैर-मुद्रण योग्य और सफेदस्थान पात्र प्रदर्शित करें (M-उपसर्ग के साथ यदि गैर-ASCII):
```shell
cat -v -t -e {{फ़ाइल}}
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/hi/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> वर्तमान कार्य निर्देशिका को बदलें।
> अधिक जानकारी: <https://man.archlinux.org/man/cd.n>.

#### दी गई निर्देशिका पर जाएं:
```shell
cd {{निर्देशिका / का / पथ}}
```
#### वर्तमान उपयोगकर्ता की होम निर्देशिका पर जाएं:
```shell
cd
```
#### वर्तमान निर्देशिका के जनक तक जाएं:
```shell
cd ..
```
#### पहले चुनी गई निर्देशिका पर जाएं:
```shell
cd -
```
{% endraw %}{% raw %}
<h2 id="chsh">
  <a href="/hi/common/chsh.html">chsh</a> <a href="#chsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> उपयोगकर्ता का लॉगिन शेल बदलें।
> अधिक जानकारी: <https://manned.org/chsh>.

#### शेल बदलें:
```shell
chsh -s {{मार्ग/का/शेल_बाइनरी}} {{उपयोगकर्ता_नाम}}
```
{% endraw %}{% raw %}
<h2 id="false">
  <a href="/hi/common/false.html">false</a> <a href="#false"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 1 का एग्जिट कोड लौटाता है।
> अधिक जानकारी: <https://www.gnu.org/software/coreutils/false>.

#### 1 का निकास कोड लौटाएँ:
```shell
false
```
{% endraw %}{% raw %}
<h2 id="git-init">
  <a href="/hi/common/git-init.html">git init</a> <a href="#git-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> एक नया स्थानीय गिट रिपॉजिटरी शुरू करता है।
> अधिक जानकारी: <https://git-scm.com/docs/git-init>।

#### एक नया स्थानीय भंडार शुरू करें:
```shell
git init
```
#### एक नंगे हड्डी के भंडार को शुरू करें, जो ssh के रिमोट के रूप में उपयोग के लिए उपयुक्त है:
```shell
git init --bare
```
{% endraw %}{% raw %}
<h2 id="ls">
  <a href="/hi/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> निर्देशिका सामग्री को सूचीबद्ध करें।
> अधिक जानकारी: <https://www.gnu.org/software/coreutils/ls>.

#### प्रति पंक्ति एक फ़ाइल की सूची बनाएं:
```shell
ls -1
```
#### छिपी हुई फाइलों सहित सभी फाइलों की सूची बनाएं:
```shell
ls -a
```
#### सभी फाइलों को सूचीबद्ध करें, '/' के साथ निर्देशिका नामों को समाप्त करें:
```shell
ls -F
```
#### सभी फ़ाइलों की लंबी प्रारूप सूची (अनुमतियाँ, स्वामित्व, आकार और परिवर्तन तिथि):
```shell
ls -la
```
#### मानव पठनीय इकाइयों (KiB, MiB, GiB) का उपयोग करके प्रदर्शित आकार के साथ लंबी प्रारूप सूची:
```shell
ls -lh
```
#### आकार के अनुसार क्रमबद्ध लंबी सूची (घटते हुए):
```shell
ls -lS
```
#### संशोधन की तारीख (सबसे पहले) द्वारा क्रमबद्ध सभी फाइलों की लंबी प्रारूप सूची:
```shell
ls -ltr
```
{% endraw %}{% raw %}
<h2 id="mkdir">
  <a href="/hi/common/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> एक निर्देशिका बनाता है।
> अधिक जानकारी: <https://www.gnu.org/software/coreutils/mkdir>.

#### वर्तमान निर्देशिका या दिए गए पथ में एक निर्देशिका बनाएँ:
```shell
mkdir {{निर्देशिका}}
```
#### निर्देशिका बनाएँ पुनरावर्ती (अंतर प्रविष्ट निर्देशिका बनाने के लिए उपयोगी):
```shell
mkdir -p {{निर्देशिका / का / पथ}}
```
{% endraw %}{% raw %}
<h2 id="time">
  <a href="/hi/common/time.html">time</a> <a href="#time"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> देखें कि एक कमांड में कितना समय लगता है।

#### समय "ls":
```shell
time ls
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/hi/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> tldr-pages प्रोजेक्ट से कमांड-लाइन टूल्स के लिए सरल हेल्प पेज प्रदर्शित करता है।
> अधिक जानकारी: https://tldr.sh

#### एक कमांड के विशिष्ट उपयोग प्राप्त करें (संकेत: इसका उपयोग कर आप यहाँ आए!):
```shell
tldr {{कमांड}}
```
#### Linux के लिए tar tldr पेज दिखाएं:
```shell
tldr -p {{linux}} {{tar}}
```
#### एक Git उपकमांड के लिए सहायता प्राप्त करें:
```shell
tldr {{git-checkout}}
```
#### स्थानीय पृष्ठों को अपडेट करें (यदि ग्राहक कैशिंग का समर्थन करता है):
```shell
tldr -u
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="view">
  <a href="/hi/common/view.html">view</a> <a href="#view"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `Vim` का केवल-पढ़ने वाला संस्करण।
> यह `विम -R` के बराबर है।

#### एक फ़ाइल खोलो:
```shell
view {{फ़ाइल}}
```
{% endraw %}