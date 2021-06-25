---
layout: default
title: "arp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp">
  <a href="/pl/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pokaż i manipuluj pamięcią podręczną ARP systemu.
> Więcej informacji: <https://manned.org/arp>.

#### Pokaż bieżącą tabelę arp:
```shell
arp -a
```
#### Wyczyść całość cache:
```shell
sudo arp -a -d
```
#### Usuń konkretny wpis:
```shell
arp -d {{adres}}
```
#### Utwórz wpis:
```shell
arp -s {{adres}} {{adres_mac}}
```
{% endraw %}