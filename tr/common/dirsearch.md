---
layout: default
title: "dirsearch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirsearch">
  <a href="/tr/common/dirsearch.html">dirsearch</a> <a href="#dirsearch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ağ yolu tarayıcı.
> Daha fazla bilgi için: <https://github.com/maurosoria/dirsearch>.

#### Bir ağ sunucusunu yaygın eklentiler içeren yaygın yollar için tarayın:
```shell
dirsearch --url {{url}} --extensions-list
```
#### Ağ sunucularını içeren bir listeyi `.php` eklentili yaygın yollar için tarayın:
```shell
dirsearch --url-list {{örnek/url-listesi.txt}} --extensions {{php}}
```
#### Bir ağ sunucusunu yaygın eklentiler içeren belirtilen yollar için tarayın:
```shell
dirsearch --url {{url}} --extensions-list --wordlist {{path/to/url-yol-listesi.txt}}
```
#### Bir ağ sunucusunu çerez kullanarak tarayın:
```shell
dirsearch --url {{url}} --extensions {{php}} --cookie {{cookie}}
```
#### Bir ağ sunucusunu `HEAD` HTTP metodunu kullanarak tarayın:
```shell
dirsearch --url {{url}} --extensions {{php}} --http-method {{HEAD}}
```
#### Bir ağ sunucusunu tarayın ve sonuçları bir `.json` dosyasına kaydedin:
```shell
dirsearch --url {{url}} --extensions {{php}} --json-report {{örnek/rapor_dosyası.json}}
```
{% endraw %}