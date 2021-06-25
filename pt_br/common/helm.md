---
layout: default
title: "helm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="helm">
  <a href="/pt_br/common/helm.html">helm</a> <a href="#helm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Helm é um gerenciador de pacores para Kubernetes.
> Mais informações: <https://helm.sh/>.

#### Cria um chart do helm:
```shell
helm create {{nome_do_chart}}
```
#### Adiciona um novo repositório helm:
```shell
helm repo add {{nome_do_repositório}}
```
#### Lista os repositórios helm:
```shell
helm repo list
```
#### Atualiza os repositórios helm:
```shell
helm repo update
```
#### Remova um repositório helm:
```shell
helm repo remove {{nome_do_repositório}}
```
#### Instala um chart helm:
```shell
helm install {{nome_do_repositório}}/{{nome_do_chart}}
```
#### Obtém um chart helm chart como um arquivo tar:
```shell
helm get {{nome_do_release_do_chart}}
```
#### Atualiza as dependências helm:
```shell
helm dependency update
```
{% endraw %}