---
layout: default
title: "mvn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mvn">
  <a href="/pt_br/common/mvn.html">mvn</a> <a href="#mvn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ferramenta para a criação e gerenciamento de projetos Java.
> Mais informações: <https://maven.apache.org/>.

#### Compilar um projeto:
```shell
mvn compile
```
#### Criar um artefato de distribuição utilizando o formato espeficado no `pom.xml`, por exemplo o formato `jar`:
```shell
mvn package
```
#### Criar um artefato de distribuição sem executar testes unitários:
```shell
mvn package -Dmaven.test.skip=true
```
#### Instalar um artefato gerado em um repositório local:
```shell
mvn install
```
#### Apagar artefatos gerados no diretório `target`:
```shell
mvn clean
```
#### Executar as fases `clean` e `package` em um projeto:
```shell
mvn clean package
```
#### Executar as fases `clean` e `package` em um projeto utilizando um perfil:
```shell
mvn clean -P{{perfil}} package
```
#### Executar uma classe que possua o método `main`:
```shell
mvn exec:java -Dexec.mainClass="{{nome.do.pacote.classe}}" -Dexec.args="{{arg1 arg2}}"
```
{% endraw %}