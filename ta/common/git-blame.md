---
layout: default
title: "git blame"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-blame">
  <a href="/ta/common/git-blame.html">git blame</a> <a href="#git-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ஒரு கோப்பின் ஒவ்வொரு வரியிலும் கமிட் ஹாஷ் மற்றும் கடைசி எழுத்தாளரைக் காட்டு.
> மேலும் தகவல்: <https://git-scm.com/docs/git-blame>.

#### எழுத்தாளர் பெயருடன் கோப்பை அச்சிட்டு ஒவ்வொரு வரியிலும் ஹாஷ் செய்யுங்கள்:
```shell
git blame {{கோப்பு}}
```
#### எழுத்தாளர் மின்னஞ்சலுடன் கோப்பை அச்சிட்டு ஒவ்வொரு வரியிலும் ஹாஷ் செய்யுங்கள்:
```shell
git blame -e {{கோப்பு}}
```
{% endraw %}