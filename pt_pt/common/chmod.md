---
layout: default
title: "chmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chmod">
  <a href="/pt_pt/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alterar as permissões de acesso a um ficheiro ou diretório.
> Mais informações: <https://www.gnu.org/software/coreutils/chmod>.

#### Dar a um [u]tilizador que possui um ficheiro o direito a e[x]ecutá-lo:
```shell
chmod u+x {{ficheiro}}
```
#### Dar a um [u]tilizador direitos para le[r] e escrever ([w]) num ficheiro/diretório:
```shell
chmod u+rw {{ficheiro_ou_diretorio}}
```
#### Remover direitos de execução de um [g]rupo:
```shell
chmod g-x {{ficheiro}}
```
#### Dar a todos ([a]) os utilizadores o direito de le[r] e e[x]ecutar:
```shell
chmod a+rx {{ficheiro}}
```
#### Dar a [o]utros (que não estão no grupo do dono do ficheiro) os mesmos direitos do [g]rupo:
```shell
chmod o=g {{ficheiro}}
```
#### Remover todos os direitos dos [o]utros:
```shell
chmod o= {{ficheiro}}
```
#### Mudar as permissões, recursivamente, dando ao [g]rupo e [o]utros a possibilidade de escrever ([w]):
```shell
chmod -R g+w,o+w {{diretorio}}
```
{% endraw %}