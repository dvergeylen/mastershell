---
layout: default
title: "kubeadm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kubeadm">
  <a href="/en/common/kubeadm.html">kubeadm</a> <a href="#kubeadm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface for creating and managing Kubernetes clusters.
> More information: <https://kubernetes.io/docs/reference/setup-tools/kubeadm>.

#### Create a Kubernetes master node:
```shell
kubeadm init
```
#### Bootstrap a Kubernetes worker node and join it to a cluster:
```shell
kubeadm join --token {{token}}
```
#### Create a new bootstrap token with a TTL of 12 hours:
```shell
kubeadm token create --ttl {{12h0m0s}}
```
#### Check if the Kubernetes cluster is upgradeable and which versions are available:
```shell
kubeadm upgrade plan
```
#### Upgrade Kubernetes cluster to a specified version:
```shell
kubeadm upgrade apply {{version}}
```
#### View the kubeadm ConfigMap containing the cluster's configuration:
```shell
kubeadm config view
```
#### Revert changes made to the host by 'kubeadm init' or 'kubeadm join':
```shell
kubeadm reset
```
{% endraw %}