---
layout: default
title: "airport"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airport">
  <a href="/es/osx/airport.html">airport</a> <a href="#airport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilidad de configuración de red inalámbrica.

#### Muestra la información del estado actual de la red inalámbrica:
```shell
airport -I
```
#### Detecta tráfico inalámbrico en el canal 1:
```shell
airport sniff {{1}}
```
#### Busca redes inalámbricas disponibles:
```shell
airport -s
```
#### Desasociarse de la red actual:
```shell
sudo airport -z
```
{% endraw %}