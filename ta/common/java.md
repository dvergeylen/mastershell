---
layout: default
title: "java"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="java">
  <a href="/ta/common/java.html">java</a> <a href="#java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ஜாவா பயன்பாட்டு துவக்கி.
> மேலும் தகவல்: <https://java.com>.

#### ஒரு main செயல்பாட்டைக் கொண்ட ஜாவா .class கோப்பை வெறும் class பெயரை பயன்படுத்தி இயக்கவும்:
```shell
java {{class_பெயரை}}
```
#### ஒரு .jar நிரலை இயக்கவும்:
```shell
java -jar {{கோபின்_பெயர்.jar}}
```
#### போர்ட் 5005 இல் இணைக்க காத்திருக்கும் பிழைதிருத்தி .jar நிரலை இயக்கவும்:
```shell
java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:5005 -jar {{கோபின்_பெயர்.jar}}
```
#### JDK, JRE மற்றும் HotSpot மென்பொருள் பதிப்புகள் காண்பி:
```shell
java -version
```
#### java கட்டளைக்கான பயன்பாட்டு தகவலை காண்பி:
```shell
java -help
```
{% endraw %}