---
layout: default
title: "fsck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fsck">
  <a href="/it/linux/fsck.html">fsck</a> <a href="#fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Controlla l'integrità di un filesystem o lo ripara. Il filesystem non dev'essere montato al momento in cui il comando viene eseguito.

#### Controlla il filesystem `/dev/sdX`, riportando eventuali blocchi danneggiati:
```shell
fsck {{/dev/sdX}}
```
#### Controlla il filesystem `/dev/sdX`, riportando eventuali blocchi danneggiati e per ognuno consente all'utente di scegliere interattivamente se ripararlo:
```shell
fsck -r {{/dev/sdX}}
```
#### Controlla il filesystem `/dev/sdX`, riportando eventuali blocchi danneggiati e riparandoli automaticamente:
```shell
fsck -a {{/dev/sdX}}
```
{% endraw %}