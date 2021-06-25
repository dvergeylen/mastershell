---
layout: default
title: "javac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="javac">
  <a href="/ta/common/javac.html">javac</a> <a href="#javac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ஜாவா நிரல்மொழிமாற்றி.

#### `.java` கோப்பை நிரல்மொழிமாற்ற:
```shell
javac {{கோப்பு.java}}
```
#### பல `.java` கோப்புகளை நிரல்மொழிமாற்ற:
```shell
javac {{கோப்பு1.java}} {{கோப்பு2.java}} {{கோப்பு3.java}}
```
#### தற்போதைய கோப்பகத்தில் அனைத்து `.java` கோப்புகளையும் நிரல்மொழிமாற்ற:
```shell
javac {{*.java}}
```
#### ஒரு `.java` கோப்பை நிரல்மொழிமாற்றி, அதன் விளைவாக வரும் `.class` கோப்பை ஒரு குறிப்பிட்ட கோப்பகத்தில் வைக்கவும்:
```shell
javac -d {{கோப்புறையை/குறிவைக்கும்/பாதை}} {{கோப்பு.java}}
```
{% endraw %}