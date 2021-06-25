---
layout: default
title: "badblocks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="badblocks">
  <a href="/it/common/badblocks.html">badblocks</a> <a href="#badblocks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cerca blocchi corrotti in un dispositivo.
> Alcuni utilizzi di badblocks possono avere esiti non reversibili, come perdita dei dati o anche della tabella delle partizioni di un disco.
> Maggiori informazioni: <https://manned.org/badblocks>.

#### Cerca blocchi corrotti in un disco utilizzando un test non distruttivo in sola lettura:
```shell
sudo badblocks {{/dev/sda}}
```
#### Cerca blocchi corrotti in un disco non montato con un test non distruttivo in lettura e scrittura:
```shell
sudo badblocks -n {{/dev/sda}}
```
#### Cerca blocchi corrotti in un disco non montato con un test distruttivo in scrittura:
```shell
sudo badblocks -w {{/dev/sda}}
```
{% endraw %}