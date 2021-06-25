---
layout: default
title: "bg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bg">
  <a href="/pt_br/common/bg.html">bg</a> <a href="#bg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retomar a execução, em segundo plano, de processos que foram suspensos (e.g. utilizando `Ctrl + Z`).
> Mais informações: <https://manned.org/bg>.

#### Retomar a execução, em segundo plano, do processo que foi suspenso mais recentemente:
```shell
bg
```
#### Retomar a execução, em segundo plano, de um processo especifico (utilizando `jobs -l` para obter o seu ID):
```shell
bg {{id_processo}}
```
{% endraw %}