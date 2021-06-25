---
layout: default
title: "dexter"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dexter">
  <a href="/it/common/dexter.html">dexter</a> <a href="#dexter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento per autenticare utenti kubectl con OpenId Connect.
> Maggiori informazioni: <https://github.com/gini/dexter>.

#### Crea ed autentica un utente con Google OIDC:
```shell
dexter auth -i {{id-client}} -s {{segreto-client}}
```
#### Sovrascrivi la posizione predefinita della configurazione di kube:
```shell
dexter auth -i {{id-client}} -s {{segreto-client}} --kube-config {{percorso/a/config}}
```
{% endraw %}