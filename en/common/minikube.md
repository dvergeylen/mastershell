---
layout: default
title: "minikube"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minikube">
  <a href="/en/common/minikube.html">minikube</a> <a href="#minikube"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to run Kubernetes locally.
> More information: <https://github.com/kubernetes/minikube>.

#### Start the cluster:
```shell
minikube start
```
#### Get the IP address of the cluster:
```shell
minikube ip
```
#### Access a service named my_service exposed via a node port and get the URL:
```shell
minikube service {{my_service}} --url
```
#### Open the Kubernetes dashboard in a browser:
```shell
minikube dashboard
```
#### Stop the running cluster:
```shell
minikube stop
```
#### Delete the cluster:
```shell
minikube delete
```
{% endraw %}