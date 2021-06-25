---
layout: default
title: "bosh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bosh">
  <a href="/en/common/bosh.html">bosh</a> <a href="#bosh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to deploy and manage the bosh director.
> More information: <https://bosh.io/docs/cli-v2/>.

#### Create local alias for director:
```shell
bosh alias-env {{environment_name}} -e {{ip_address|url}} --ca-cert {{ca_certificate}}
```
#### List environments:
```shell
bosh environments
```
#### Log in to the director:
```shell
bosh login -e {{environment}} 
```
#### List deployments:
```shell
bosh -e {{environment}} deployments
```
#### List environment virtual machines:
```shell
bosh -e {{environment}} vms -d {{deployment}}
```
#### Ssh into virtual machine:
```shell
bosh -e {{environment}} ssh {{virtual_machine}} -d {{deployment}}
```
#### Upload stemcell:
```shell
bosh -e {{environment}} upload-stemcell {{stemcell_file|url}}
```
#### Show current cloud config:
```shell
bosh -e {{environment}} cloud-config
```
{% endraw %}