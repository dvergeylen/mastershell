---
layout: default
title: "command"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="command">
  <a href="/tr/common/command.html">command</a> <a href="#command"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command, kabuğu bir programı herhangi bir fonksiyon ve gömülü özelliğe ve alias'a takılmadan çalıştırmaya zorlar.
> Daha fazla bilgi için: <https://manned.org/command>.

#### `ls` programını aynı isimde bir alias olsa dahi çalıştır:
```shell
command {{ls}}
```
#### Alias'a atanan özel komutu veya çalıştırılabilir dosyanın yolunu göster:
```shell
command -v {{komut_ismi}}
```
{% endraw %}