---
layout: default
title: "pidof"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pidof">
  <a href="/it/linux/pidof.html">pidof</a> <a href="#pidof"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ottiene l'ID di un processo a partire dal suo nome.

#### Elenca gli ID di tutti i processi con un dato nome:
```shell
pidof {{bash}}
```
#### Elenca un solo ID di processo con il nome specificato:
```shell
pidof -s {{bash}}
```
#### Elenca gli ID dei processi con un dato includendo anche gli script:
```shell
pidof -x {{script.py}}
```
#### Uccide tutti i processi con un dato nome:
```shell
kill "$(pidof {{nome}})" 
```
{% endraw %}