---
layout: default
title: "gh secret set"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gh-secret-set">
  <a href="/en/common/gh-secret-set.html">gh secret set</a> <a href="#gh-secret-set"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create or update GitHub secrets from the command line.
> More information: <https://cli.github.com/manual/gh_secret_set>.

#### Set a secret for the current repository (user will be prompted for the value):
```shell
gh secret set {{name}}
```
#### Set a secret from a file for the current repository:
```shell
gh secret set {{name}} < {{path/to/file}}
```
#### Set a secret for a specific repository:
```shell
gh secret set {{name}} --body {{value}} --repo {{owner}}/{{repository}}
```
#### Set an organization secret for specific repositories:
```shell
gh secret set {{name}} --org {{organization}} --repos "{{repository1,repository2,...}}"
```
#### Set an organization secret with a specific visibility:
```shell
gh secret set {{name}} --org {{organization}} --visibility {{all|private|selected}}
```
{% endraw %}