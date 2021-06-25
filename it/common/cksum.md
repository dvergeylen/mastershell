---
layout: default
title: "cksum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cksum">
  <a href="/it/common/cksum.html">cksum</a> <a href="#cksum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calcola checksum CRC e conta i byte di un file.
> Nota: in vecchi sistemi UNIX l'implementazione di CRC potrebbe essere diversa.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/cksum>.

#### Calcola e mostra un checksum di 32 bit, dimensione in byte e nome del file:
```shell
cksum {{percorso/al/file}}
```
{% endraw %}