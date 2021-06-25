---
layout: default
title: "git cat-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cat-file">
  <a href="/ta/common/git-cat-file.html">git cat-file</a> <a href="#git-cat-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> கிட் களஞ்சிய பொருள்களுக்கான உள்ளடக்கம் அல்லது வகை மற்றும் அளவு தகவல்களை வழங்கவும்.
> மேலும் தகவல்: <https://git-scm.com/docs/git-cat-file>.

#### HEAD கமிட்டின் அளவை பைட்டுகளில் பெறுங்கள்:
```shell
git cat-file -s HEAD
```
#### கொடுக்கப்பட்ட கிட் பொருளின் வகையை (குமிழ், மரம், கமிட், டேக்) பெறுங்கள்:
```shell
git cat-file -t {{8c442dc3}}
```
#### கொடுக்கப்பட்ட கிட் பொருளின் உள்ளடக்கத்தை அதன் வகையின் அடிப்படையில் அழகாக அச்சிடுக:
```shell
git cat-file -p {{HEAD~2}}
```
{% endraw %}