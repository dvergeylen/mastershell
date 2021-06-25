---
layout: default
title: "bosh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bosh">
  <a href="/it/common/bosh.html">bosh</a> <a href="#bosh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento da linea di comando per distribuire e gestire director BOSH.
> Maggiori informazioni: <https://bosh.io/docs/cli-v2/>.

#### Crea un alias locale per un director:
```shell
bosh alias-env {{nome_ambiente}} -e {{indirizzo_ip|url}} --ca-cert {{certificato_ca}}
```
#### Elenca ambienti:
```shell
bosh environments
```
#### Esegui il login al director:
```shell
bosh login -e {{ambiente}} 
```
#### Elenca deployment (distribuzioni):
```shell
bosh -e {{ambiente}} deployments
```
#### Elenca le macchine virtuali in un ambiente:
```shell
bosh -e {{ambiente}} vms -d {{deployment}}
```
#### Avvia una sessione SSH in una macchina virtuale:
```shell
bosh -e {{ambiente}} ssh {{macchina_virtuale}} -d {{deployment}}
```
#### Carica una stemcell:
```shell
bosh -e {{ambiente}} upload-stemcell {{file_stemcell|url}}
```
#### Mostra la configurazione cloud attuale:
```shell
bosh -e {{ambiente}} cloud-config
```
{% endraw %}