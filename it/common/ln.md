---
layout: default
title: "ln"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ln">
  <a href="/it/common/ln.html">ln</a> <a href="#ln"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea un collegamento a un file o a una directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/ln>.

#### Crea un collegamento simbolico a un file (o directory):
```shell
ln -s {{/percorso/al/file}} {{percorso/al/collegamento}}
```
#### Sovrascrivi un collegamento esistente in modo che punti a un nuovo file:
```shell
ln -sf {{/percorso/al/nuovo/file}} {{percorso/al/collegamento}}
```
#### Crea un collegamento fisico a un file:
```shell
ln {{/percorso/al/file}} {{percorso/al/collegamento}}
```
{% endraw %}