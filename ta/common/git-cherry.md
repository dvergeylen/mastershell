---
layout: default
title: "git cherry"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cherry">
  <a href="/ta/common/git-cherry.html">git cherry</a> <a href="#git-cherry"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> அப்ஸ்ட்ரீமில் இன்னும் பயன்படுத்தப்படாத கமிட்டுகளைக் கண்டறியவும்.
> மேலும் தகவல்: <https://git-scm.com/docs/git-cherry>.

#### அப்ஸ்ட்ரீமில் சமமான கமிட்டுகளுடன் கமிட்டுகளையும் (அவற்றின் செய்திகளையும்) காட்டு:
```shell
git cherry -v
```
#### வேறு அப்ஸ்ட்ரீம் மற்றும் தலைப்பு கிளையை குறிப்பிடவும்:
```shell
git cherry {{தோற்றம்}} {{தலைப்பு}}
```
#### கொடுக்கப்பட்ட வரம்புக்குள் கமிட்களை கட்டுப்படுத்து:
```shell
git cherry {{தோற்றம்}} {{தலைப்பு}} {{அடித்தளம்}}
```
{% endraw %}