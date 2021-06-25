---
layout: default
title: "xfce4-terminal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xfce4-terminal">
  <a href="/tr/linux/xfce4-terminal.html">xfce4-terminal</a> <a href="#xfce4-terminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> XFCE4 terminal öykünücüsü.
> Daha fazla bilgi için: <https://docs.xfce.org/apps/xfce4-terminal/start>.

#### Yeni bir terminal penceresi aç:
```shell
xfce4-terminal
```
#### Başlangıç başlığı belirle:
```shell
xfce4-terminal --initial-title "{{başlangıç_başlığı}}"
```
#### Mevcut terminal penceresinde yeni bir sekme aç:
```shell
xfce4-terminal --tab
```
#### Yeni bir terminal penceresini belirlenen bir komutu çalıştırarak aç:
```shell
xfce4-terminal --command "{{argümanlı_komut}}"
```
#### Çalıştırılan komutun çalışmayı kesme durumunda dahi terminali kapama:
```shell
xfce4-terminal --command "{{argümanlı_komut}}" --hold
```
#### Her birinde farklı komut çalışacak birçok yeni sekme aç:
```shell
xfce4-terminal --tab --command "{{komut_a}}" --tab --command "{{komut_b}}"
```
{% endraw %}