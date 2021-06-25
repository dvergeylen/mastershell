---
layout: default
title: "touch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="touch">
  <a href="/pt_br/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Atualizar as timestamps de um arquivo para a hora atual.
> Se o arquivo não existir, cria um arquivo vazio, a menos que seja passado o parâmetro -c ou -h.
> Mais informações: <https://www.gnu.org/software/coreutils/touch>.

#### Criar um novo arquivo vazio, ou atualizar as timestamps para a hora atual:
```shell
touch {{arquivo}}
```
#### Definir as timestamps de um arquivo para a hora especificada:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{arquivo}}
```
#### Usar as timestamps do arquivo1 para definir as timestamps do arquivo2:
```shell
touch -r {{arquivo1}} {{arquivo2}}
```
#### Alterar as timestamps de um arquivo. Não cria novo arquivo se não existir:
```shell
touch -c {{arquivo}}
```
{% endraw %}