---
layout: default
title: "touch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="touch">
  <a href="/pt_pt/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Atualizar as timestamps de um ficheiro para a hora atual.
> Se o ficheiro não existir, cria um ficheiro vazio, a menos que seja passado o parâmetro -c ou -h.
> Mais informações: <https://www.gnu.org/software/coreutils/touch>.

#### Criar um novo ficheiro vazio, ou atualizar as timestamps para a hora atual:
```shell
touch {{ficheiro}}
```
#### Definir as timestamps de um ficheiro para a hora especificada:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{ficheiro}}
```
#### Usar as timestamps do ficheiro1 para definir as timestamps do ficheiro2:
```shell
touch -r {{ficheiro1}} {{ficheiro2}}
```
#### Alterar as timestamps de um ficheiro. Não cria novo ficheiro se não existir:
```shell
touch -c {{ficheiro}}
```
{% endraw %}