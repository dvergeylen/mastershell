---
layout: default
title: "git bundle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-bundle">
  <a href="/ta/common/git-bundle.html">git bundle</a> <a href="#git-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ஒரு காப்பக கோப்பில் பொருள்கள் மற்றும் குறிப்புகளை தொகுக்கவும்.
> மேலும் தகவல்: <https://git-scm.com/docs/git-bundle>.

#### ஒரு குறிப்பிட்ட கிளையின் அனைத்து பொருள்கள் மற்றும் குறிப்புகளைக் கொண்ட ஒரு மூட்டை கோப்பை உருவாக்கவும்:
```shell
git bundle create {{கோப்புக்கான/பாதை/கோப்பு.bundle}} {{கிளையின்_பெயர்}}
```
#### அனைத்து கிளைகளின் மூட்டை கோப்பை உருவாக்கவும்:
```shell
git bundle create {{கோப்புக்கான/பாதை/கோப்பு.bundle}} --all
```
#### தற்போதைய கிளையின் கடைசி 5 கமிட்டுகளின் மூட்டை கோப்பை உருவாக்கவும்:
```shell
git bundle create {{கோப்புக்கான/பாதை/கோப்பு.bundle}} -{{5}} {{HEAD}}
```
#### சமீபத்திய 7 நாட்களின் மூட்டை கோப்பை உருவாக்கவும்:
```shell
git bundle create {{கோப்புக்கான/பாதை/கோப்பு.bundle}} --since={{7.days}} {{HEAD}}
```
#### ஒரு மூட்டை கோப்பு தற்போதைய களஞ்சியத்தில் செல்லுபடியாகும் மற்றும் பயன்படுத்தலாம் என்பதை சரிபார்க்கவும்:
```shell
git bundle verify {{கோப்புக்கான/பாதை/கோப்பு.bundle}}
```
#### ஒரு மூட்டையில் உள்ள குறிப்புகளின் பட்டியலை நிலையான வெளியீட்டில் அச்சிடுக:
```shell
git bundle unbundle {{கோப்புக்கான/பாதை/கோப்பு.bundle}}
```
#### ஒரு மூட்டை கோப்பிலிருந்து ஒரு குறிப்பிட்ட கிளையை தற்போதைய களஞ்சியத்தில் இணைக்கவும்:
```shell
git pull {{கோப்புக்கான/பாதை/கோப்பு.bundle}} {{கிளையின்_பெயர்}}
```
{% endraw %}