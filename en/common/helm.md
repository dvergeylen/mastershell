---
layout: default
title: "helm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="helm">
  <a href="/en/common/helm.html">helm</a> <a href="#helm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Helm is a package manager for Kubernetes.
> More information: <https://helm.sh/>.

#### Create a helm chart:
```shell
helm create {{chart_name}}
```
#### Add a new helm repository:
```shell
helm repo add {{repo_name}}
```
#### List helm repositories:
```shell
helm repo list
```
#### Update helm repositories:
```shell
helm repo update
```
#### Delete a helm repository:
```shell
helm repo remove {{repo_name}}
```
#### Install a helm chart:
```shell
helm install {{repo_name}}/{{chart_name}}
```
#### Download helm chart as a tar archive:
```shell
helm get {{chart_release_name}}
```
#### Update helm dependencies:
```shell
helm dependency update
```
{% endraw %}