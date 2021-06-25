---
layout: default
title: "gpg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gpg">
  <a href="/pt_br/common/gpg.html">gpg</a> <a href="#gpg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard.
> Mais informações: <https://gnupg.org>.

#### Assina doc.txt, sem criptografá-lo (cria um arquivo de saída doc.txt.asc):
```shell
gpg --clearsign {{doc.txt}}
```
#### Criptografa doc.txt para alice@example.com (cria um arquivo de saída `doc.txt.gpg`):
```shell
gpg --encrypt --recipient {{alice@example.com}} {{doc.txt}}
```
#### Criptografa doc.txt apenas com uma senha simétrica (cria um arquivo de sadída `doc.txt.gpg`):
```shell
gpg --symmetric {{doc.txt}}
```
#### Descriptografa doc.txt.gpg (envia saída para stdout):
```shell
gpg --decrypt {{doc.txt.gpg}}
```
#### Importa uma chave pública:
```shell
gpg --import {{public.gpg}}
```
#### Exporta a chave pública da alice@example.com (envia saída para stdout):
```shell
gpg --export --armor {{alice@example.com}}
```
#### Exporta chave privada da alice@example.com (envia saída para stdout):
```shell
gpg --export-secret-keys --armor {{alice@example.com}}
```
{% endraw %}