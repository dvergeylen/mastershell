---
layout: default
title: "dhcpwn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dhcpwn">
  <a href="/ko/common/dhcpwn.html">dhcpwn</a> <a href="#dhcpwn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DHCP IP 소진하는 공격을 테스트하고 로컬 DHCP 트래픽을 스니핑한다.
> 더 많은 정보: <https://github.com/mschwager/dhcpwn>.

#### 네트워크에 IP 요청들로 쇄도하기:
```shell
dhcpwn --interface {{네트워크_인터페이스}} flood --count {{요청들의_수}}
```
#### 로컬 DHCP 트래픽 스니핑하기:
```shell
dhcpwn --interface {{네트워크_인터페이스}} sniff
```
{% endraw %}