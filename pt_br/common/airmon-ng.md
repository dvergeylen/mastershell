---
layout: default
title: "airmon-ng"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airmon-ng">
  <a href="/pt_br/common/airmon-ng.html">airmon-ng</a> <a href="#airmon-ng"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ativa modo de monitoramento em dispositivos de rede sem-fio.
> Mais informações: <https://www.aircrack-ng.org/doku.php?id=airmon-ng>.

#### Lista os dispositivos sem-fio e seus respectivos estados:
```shell
sudo airmon-ng
```
#### Liga o modo de monitoramento para um dispositivo específico:
```shell
sudo airmon-ng start {{wlan0}}
```
#### Encerra processos problemáticos que usam dispositivos sem-fio:
```shell
sudo airmon-ng check kill
```
#### Desativa o modo de monitoramento para um dispositivo específico:
```shell
sudo airmon-ng stop {{wlan0mon}}
```
{% endraw %}