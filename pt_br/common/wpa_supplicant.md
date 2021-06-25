---
layout: default
title: "wpa_supplicant"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wpa_supplicant">
  <a href="/pt_br/common/wpa_supplicant.html">wpa_supplicant</a> <a href="#wpa_supplicant"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gerenciador de redes wireless protegidas.

#### Entrar em uma rede wireless protegida:
```shell
wpa_supplicant -i {{interface}} -c {{caminho/para/wpa_supplicant_conf.conf}}
```
#### Entrar em uma rede wireless protegida e executar o wpa_cli em um daemon:
```shell
wpa_supplicant -B -i {{interface}} -c {{caminho/para/wpa_supplicant_conf.conf}}
```
{% endraw %}