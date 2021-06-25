---
layout: default
title: "gh secret"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-secret">
  <a href="/en/common/gh-secret.html">gh secret</a> <a href="#gh-secret"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage GitHub secrets from the command-line.
> More information: <https://cli.github.com/manual/gh_secret>.

#### List secret keys for the current repository:
```shell
gh secret list
```
#### List secret keys for a specific organization:
```shell
gh secret list --org {{organization}}
```
#### List secret keys for a specific repository:
```shell
gh secret list --repo {{owner}}/{{repository}}
```
#### Set a secret for the current repository (user will be prompted for the value):
```shell
gh secret set {{name}}
```
#### Set a secret from a file for the current repository:
```shell
gh secret set {{name}} < {{path/to/file}}
```
#### Set an organization secret for specific repositories:
```shell
gh secret set {{name}} --org {{organization}} --repos {{repository1,repository2}}
```
#### Remove a secret for the current repository:
```shell
gh secret remove {{name}}
```
#### Remove a secret for a specific organization:
```shell
gh secret remove {{name}} --org {{organization}}
```
{% endraw %}