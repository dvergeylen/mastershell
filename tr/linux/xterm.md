---
layout: default
title: "xterm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xterm">
  <a href="/tr/linux/xterm.html">xterm</a> <a href="#xterm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> X Ekran Sistemi için terminal öykünücüsü.

#### `Örnek` başlığına sahip bir terminal aç:
```shell
xterm -T {{Örnek}}
```
#### Terminali tam ekran modunda aç:
```shell
xterm -fullscreen
```
#### Terminali lacivert arkaplan ve sarı ön plan (font rengi) ile aç:
```shell
xterm -bg {{darkblue}} -fg {{yellow}}
```
#### Terminali satır başına 100 karakter ve sütun başına 35 satır sığacak şekilde, x=200px y=20px koordinatlarında aç:
```shell
xterm -geometry {{100}}x{{35}}+{{200}}+{{20}}
```
#### Terminali bir Serif fontu ve 20'ye eşit olan bir font büyüklüğü ile aç:
```shell
xterm -fa "{{Serif}}" -fs {{20}}
```
{% endraw %}