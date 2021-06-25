---
layout: default
title: "dhclient"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dhclient">
  <a href="/ko/common/dhclient.html">dhclient</a> <a href="#dhclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DHCP 클라이언트.
> 더 많은 정보: <https://manned.org/dhclient>.

#### 'eht0' 인터페이스의 IP 주소 얻기:
```shell
sudo dhclient {{eth0}}
```
#### 'eth0' 인터페이스의 IP 주소 해제하기:
```shell
sudo dhclient -r {{eth0}}
```
{% endraw %}