---
layout: default
title: "git clean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clean">
  <a href="/ta/common/git-clean.html">git clean</a> <a href="#git-clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> கண்காணிக்கப்படாத கோப்புகளை பணியிடத்திலிருந்து அகற்றவும்.
> மேலும் தகவல்: <https://git-scm.com/docs/git-clean>.

#### கிட் மூலம் கண்காணிக்கப்படாத கோப்புகளை நீக்கு:
```shell
git clean
```
#### கிட் மூலம் கண்காணிக்கப்படாத கோப்புகளை ஊடாடும் வகையில் நீக்கு:
```shell
git clean -i
```
#### எந்த கோப்புகள் உண்மையில் நீக்கப்படாமல் நீக்கப்படும் என்பதைக் காட்டு:
```shell
git clean --dry-run
```
#### கிட் மூலம் கண்காணிக்கப்படாத கோப்புகளை கட்டாயமாக நீக்கு:
```shell
git clean -f
```
#### கிட் மூலம் கண்காணிக்கப்படாத கோப்பகங்களை கட்டாயமாக நீக்கு:
```shell
git clean -fd
```
#### `.gitignore` மற்றும் `.git/info/exclude` ஆகியவற்றில் புறக்கணிக்கப்பட்ட கோப்புகள் உட்பட, தடமறியப்படாத கோப்புகளை நீக்கு:
```shell
git clean -x
```
{% endraw %}