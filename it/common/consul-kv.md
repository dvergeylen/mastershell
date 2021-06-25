---
layout: default
title: "consul-kv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="consul-kv">
  <a href="/it/common/consul-kv.html">consul-kv</a> <a href="#consul-kv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rete distribuita per gestire e configurare servizi tramite database chiave-valore.
> Maggiori informazioni: <https://learn.hashicorp.com/consul/getting-started/kv>.

#### Leggi il valore di una chiave da un database chiave-valore:
```shell
consul kv get {{chiave}}
```
#### Memorizza una nuova coppia chiave-valore:
```shell
consul kv put {{chiave}} {{valore}}
```
#### Elimina una coppia chiave-valore:
```shell
consul kv delete {{chiave}}
```
{% endraw %}