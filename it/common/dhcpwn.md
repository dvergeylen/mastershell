---
layout: default
title: "dhcpwn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dhcpwn">
  <a href="/it/common/dhcpwn.html">dhcpwn</a> <a href="#dhcpwn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Testa attacchi di esaurimento IP DHCP ed intercetta il traffico DHCP locale.
> Maggiori informazioni: <https://github.com/mschwager/dhcpwn>.

#### Inonda la rete con richieste di IP:
```shell
dhcpwn --interface {{interfaccia}} flood --count {{numero_di_richieste}}
```
#### Intercetta traffico DHCP locale:
```shell
dhcpwn --interface {{interfaccia}} sniff
```
{% endraw %}