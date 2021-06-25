---
layout: default
title: "vela"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vela">
  <a href="/en/common/vela.html">vela</a> <a href="#vela"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tools for the Vela pipeline.
> More information: <https://go-vela.github.io/docs/cli/>.

#### Trigger a pipeline to run from a Git branch, commit or tag:
```shell
vela add deployment --org {{organization}} --repo {{repository_name}} --target {{environment}} --ref {{branch|commit|refs/tags/git_tag}} --description "{{deploy_description}}"
```
#### List deployments for a repository:
```shell
vela get deployment --org {{organization}} --repo {{repository_name}}
```
#### Inspect a specific deployment:
```shell
vela view deployment --org {{organization}} --repo {{repository_name}} --deployment {{deployment_number}}
```
{% endraw %}