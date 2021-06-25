---
layout: default
title: "git apply"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-apply">
  <a href="/ta/common/git-apply.html">git apply</a> <a href="#git-apply"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> கோப்புகள் மற்றும் / அல்லது குறியீட்டுக்கு ஒரு இணைப்பு பயன்படுத்தவும்.
> மேலும் தகவல்: <https://git-scm.com/docs/git-apply>.

#### இணைக்கப்பட்ட கோப்புகளைப் பற்றிய செய்திகளை அச்சிடுங்கள்:
```shell
git apply --verbose {{கோப்புக்கான/பாதை}}
```
#### இணைக்கப்பட்ட கோப்புகளை குறியீட்டில் பயன்படுத்தவும் மற்றும் சேர்க்கவும்:
```shell
git apply --index {{கோப்புக்கான/பாதை}}
```
#### ரிமோட் பேட்ச் கோப்பைப் பயன்படுத்துங்கள்:
```shell
curl {{https://example.com/கோப்பு.patch}} | git apply
```
#### உள்ளீட்டிற்கான வெளியீட்டு வேறுபாடு நிலை மற்றும் இணைப்பு பொருந்தும்:
```shell
git apply --stat --apply {{கோப்புக்கான/பாதை}}
```
#### பேட்சை தலைகீழாகப் பயன்படுத்துங்கள்:
```shell
git apply --reverse {{கோப்புக்கான/பாதை}}
```
#### பேட்ச் முடிவை குறியீட்டில் வேலை செய்யும் மரத்தை மாற்றாமல் சேமிக்கவும்:
```shell
git apply --cache {{கோப்புக்கான/பாதை}}
```
{% endraw %}