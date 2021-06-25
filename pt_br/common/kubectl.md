---
layout: default
title: "kubectl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kubectl">
  <a href="/pt_br/common/kubectl.html">kubectl</a> <a href="#kubectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Linha de comando para executar comando em clusters do Kubernetes.
> Mais informações: <https://kubernetes.io/docs/reference/kubectl/>.

#### Lista toda a informação sobre um recurso em detalhes:
```shell
kubectl get {{pod|service|deployment|ingress|...}} -o wide
```
#### Atualiza um pod específico com o label 'unhealthy' e o valor 'true':
```shell
kubectl label pods {{name}} unhealthy=true
```
#### Lista todos os recursos de diferentes tipos:
```shell
kubectl get all
```
#### Exibe os usos de recursos (CPU/Memória/Espaço alocado) dos nós ou pods:
```shell
kubectl top {{pod|node}}
```
#### Exibe os endereços dos serviços do master e do cluster:
```shell
kubectl cluster-info
```
#### Exibe uma explicação de um campo específico:
```shell
kubectl explain {{pods.spec.containers}}
```
#### Exibe os logs de um container em um pod ou de um recurso específico:
```shell
kubectl logs {{pod_name}}
```
#### Executa um comando em um pod existente:
```shell
kubectl exec {{pod_name}} -- {{ls /}}
```
{% endraw %}