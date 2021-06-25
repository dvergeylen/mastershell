---
layout: default
title: "detox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="detox">
  <a href="/it/common/detox.html">detox</a> <a href="#detox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rinomina file per renderli facili da utilizzare.
> Rimuove spazi e altri caratteri fastidiosi come doppi caratteri underline.
> Maggiori informazioni: <https://github.com/dharple/detox>.

#### Rimuovi spazi ed altri caratteri indesiderabili dal nome di un file:
```shell
detox {{file}}
```
#### Mostra come detox rinominerebbe tutti i file in una directory ricorsivamente:
```shell
detox --dry-run -r {{directory}}
```
#### Rimuovi spazi e altri caratteri indesiderabili da tutti i file in una directory ricorsivamente:
```shell
detox -r {{directory}}
```
{% endraw %}