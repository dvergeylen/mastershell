---
layout: default
title: "kustomize"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kustomize">
  <a href="/en/common/kustomize.html">kustomize</a> <a href="#kustomize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kustomize is a tool to easily deploy resources for Kubernetes.
> More information: <https://github.com/kubernetes-sigs/kustomize>.

#### Create kustomization file with resources and namespace:
```shell
kustomize create --resources {{deployment.yaml,service.yaml}} --namespace {{staging}}
```
#### Build kustomization file and deploy it with `kubectl`:
```shell
kustomize build . | kubectl apply -f -
```
#### Set an image in the kustomization file:
```shell
kustomize edit set image {{busybox=alpine:3.6}}
```
#### Search for Kubernetes resources in the current directory to be added to the kustomization file:
```shell
kustomize create --autodetect
```
{% endraw %}