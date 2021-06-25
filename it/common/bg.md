---
layout: default
title: "bg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bg">
  <a href="/it/common/bg.html">bg</a> <a href="#bg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Riprende job che sono stati sospesi (e.g. usando `Ctrl + Z`) mettendoli in esecuzione in background.
> Maggiori informazioni: <https://manned.org/bg>.

#### Riprendi il job sospeso più recentemente ed eseguilo in background:
```shell
bg
```
#### Riprendi uno specifico job (usa `jobs -l` per trovare l'ID) ed eseguilo in background:
```shell
bg {{id_job}}
```
{% endraw %}